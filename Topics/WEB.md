### 홈페이지가 사용자에게 보이는 순서
  - 클라이언트가 URL통해 서버에 요청한다.
  - DNS를 통해 실제 서버에 요청이 된다.
  - 서버는 HTML 문서를 응답해 준다.
  - 클라이언트 측의 브라우저는 응답받은 HTML 문서 데이터를 파싱한다.
  - HTML문서를 파싱하여 DOM Tree를 만들어 낸다.
  - 파싱 중 Javascript 태그를 만나면 javascript 실행까지 멈추었다가 파싱을 진행한다.
  - 파싱 중 CSS 링크를 만나면, CSS파일을 요청해 받아온다.
  - CSSOM (CSS Object Model)을 만든다.
  - DOM tree 와 CSSOM 을 사용해 화면에 보여지게될 노드들로 구성되어있는 Render Tree를 생성한다.
  - Layout 구성 단계: Render Tree에 구성된 노드들이 실제로 보여질 위치와 크기를 계산한여, 렌더 트리를 배치한다.
  - Paint 단계: 구성된 Layout기반으로 UI 백엔드를 통해 화면에 출력한다.
![Image](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/images/render-tree-construction.png?hl=ko)
