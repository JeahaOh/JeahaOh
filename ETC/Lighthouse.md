# Google Lighthouse

구글에서 제공하는 웹페이지 품질 개선을 위항 오픈 소스 자동화 툴.  
성능, 접근성, 권장사항, SEO, PWA 에 대한 검사 가능.  

## 중요 측정 항목

- FCP (First Contentful Paint)  
  - 페이지 로드가 시작된 시점부터 페이지 콘텐츠의 일부가 화면에 렌더링되는 시점까지의 시간 측정.
  - 1.8초 이하 권장
  - [FCP](https://web.dev/articles/fcp?hl=ko)
- LCP (Lagest Contentful Paint)  
  - 페이지가 로드되기 시작한 시점부터 가장 큰 텍스트 믈록 또는 이미지 요소가 화면에 렌더링되는 시점 까지의 시간 측정.
  - 2.5초 이하 권장
  - [LCP](https://web.dev/articles/lcp?hl=ko)
- INP (Interaction to Next Paint)  
  - 페이지에서 이루어지는 모든 탭, 클릭, 키보드 상호작용의 지연 시간.
  - 상소작용 수를 기반으로 페이지의 최악 상호작용 지연시간을 페이지의 전반적인 응답성으로 판단.
  - [INP](https://web.dev/articles/inp?hl=ko)
- TBT (Total Blocking Time)  
  - 사용자가 화면에서 페이지를 이용(상호작용)할 수 있기 전까지 브라우져가 상호작용을 차단하는 시간.
  - 50 ms 권장
  - [TBT](https://web.dev/articles/tbt?hl=ko)
- CLS (Cumulative Layout Shift)  
  - 레이아웃 변경 횟수.  
  - 콘텐츠 로딩으로 인해 사용자가 읽던 위치를 잃거나 잘못된 링크 또는 버튼을 클릭하게 되는 레이아웃의 변경 횟수.
  - 0.1 점 이하 권장
  - [CLS](https://web.dev/articles/cls?hl=ko)
- TTFB (Time to First Byte)    
  - 리소스 요청과 응답의 첫 번째 바이트가 도달하는 시작점간의 시간의 측정도.
  - [TTFB](https://web.dev/articles/ttfb?hl=ko)


## 결과 요약 항목

- Performance : 웹페이지의 로딩 속도와 같은 성능 측정.
- Accessibility : 접근성 지표 (버튼 간의 간격이나 글 폰트 싸이즈 등)
- Best Practices : 권장 사항을 따라 개발되었는지 확인.
- SEO (Search Engine Optimization) : 검색엔진 최적화 지표.
- PWA (Progressive Web App) : 웹과 네이티브 앱의 기능 모두 이점을 가지도록 만들어진 서비스인지 확인.

