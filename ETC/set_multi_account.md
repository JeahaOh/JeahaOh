# 한 컴퓨터에서 Github 계정 여러개 사용하기

<!-- github config ssh 계정 multiple account 두개 분리 여러 관리-->

회사와 개인프로젝트의 계정을 분리한다던지, 개인 프로젝트와 스터디 그룹의 계정을 분리한다던지 한 컴퓨터에서 여러 Github 계정을 사용해야 할 경우가 있다.  SSH를 활용하여 관리하는 방법을 사용하면 편하다.  

## 기존에 ssh 키가 있는지 확인

```shell
  ls -al ~/.ssh
```

## ssh 키를 생성 및 agent 등록

```shell
  # 2개의 키 생성하기
  ssh-keygen -t rsa -C "{private}@mail.com" -f "~/.ssh/{rsa file for private}"
  ssh-keygen -t rsa -C "{group}@mail.com" -f "~/.ssh/{rsa file for group}"

  # 키 생성 확인
  ls -al ~/.ssh

  # ssh-agent 실행 확인
  eval "$(ssh-agent -s)"

  # 생성한 키 등록
  ssh-add ~/.ssh/{rsa file for private}
  ssh-add ~/.ssh/{rsa file for group}

  # 등록한 키 확인
  ssh-add -l
  4096 SHA256:... {private}@mail.com (RSA)
  4096 SHA256:... {group}@mail.com (RSA)
```

## ssh 설정 파일 수정

ssh 설정 파일은 `~/.ssh/config`이다. 파일이 존재하지 않는다면 생성 후 진행한다.

```shell
  # 파일 존재 여부 확인
  cat ~/.ssh/config

  # 파일 생성
  touch ~/.ssh/config

  # 파일 수정
  vi ~/.ssh/config
```

```shell
  # IDLOOK
  Host github.com-{group_name}
    HostName github.com    
    User {group_github_name}
    IdentityFile ~/.ssh/{rsa file for group}

  # PRIVATE
  Host github.com-{private_name}
    HostName github.com
    User {private_github_name}
    IdentityFile ~/.ssh/{rsa file for private}
```

## git 설정파일 수정

git user name과 user email 설정 파일을 각각 생성 수정한다

```shell
  touch ~/.gitconfig-{private}
  touch ~/.gitconfig-{group}
```

### 개인용

```shell
  vi ~/.gitconfig-{private}
```
```shell
  [user]
    name = {private_github_name}
    email = {private}@mail.com
```

### 업무용

```shell
  vi ~/.gitconfig-{group}
```
```shell
  [user]
    name = {group_github_name}
    email = {group}@mail.com
```

### git 설정 파일에서 해당 파일을 읽어오도록 한다

```shell
  vi ~/.gitconfig
```

```shell
  [includeIf "gitdir:{개인 프로젝트 경로}"]
    path = .gitconfig-{private}
  [includeIf "gitdir:{그룹 프로젝트 경로}"]
    path = .gitconfig-{group}
```

## Github 계정에 SSH 키를 등록

생성한 ssh 키를 각각 두개의 github 계정에 등록해준다.
  
우측 상단 Github Profile > Settings > 좌측 SSH and GPG keys > 우측상단 New SSH Key  
타이틀은 편하게, Key type은 Authentication Key, Key 부분에 생성한 키를 복사해서 붙여 넣는다.

```shell
  # shell에서 명령어로 복사하는 방법
  pbcopy < ~/.ssh/{rsa file for private}

  # shell에서 명령어로 출력한 후 terminal에서 복사하는 방법
  cat ~/.ssh/{rsa file for private}
```

## Github 등록 확인

```shell
  ssh -T git@github.com-{private_name}
```

## 로컬로 Github 레포지토리 복사

복사시 https가 아닌 ssh로 한다

```shell
  git clone git@github.com-{private_name}:{user-name}/{repository-name}.git
```

## 로컬이 이미 레포지토리가 있을 경우 주소 변경

```shell
  # 기존 리모트 url 확인
  git config --get remote.origin.url
  git@github.com:{A}/{B}.git
  # 리모트 url 변경
  git remote set-url origin git@github.com-{private_name}:{A}/{B}.git

  # 동작 확인
  git pull
```

## clone, pull등 git 명령어 결과에서 에러가 나올 경우 ssh를 디버깅 모드로 시도

```shell
  GIT_SSH_COMMAND="ssh -v" git fetch
```

## DL;DR

모든 내용은 git manual에 있다.https://git-scm.com/docs/git-config#_conditional_includes


### 참고

- https://git-scm.com/docs/git-config#_includes
- https://git-scm.com/docs/git-config#_conditional_includes
- https://www.lesstif.com/gitbook/git-ssh-verbose-mode-125305437.html