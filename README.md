# html 템플릿 분리하기
출처 : (vleg)[https://kay0426.tistory.com/27?category=789875]

## 템플릿 사용법
### Load Content
하나의 파일에서 `header`, `content`, `footer`를 로드하여, 메뉴 클릭 시 content의 내용을 업데이트 하는 식으로 보여준다

해당 내용은 실 반영페이지를 보기에 적합하며, 링크를 확인하기에 편리하다. 하지만 개발자나 신규 작업자가 해당 프로젝트 분석시, 파일을 헷갈릴 우려가 있다.

또한 페이지마다 레이아웃이 다르거나, 팝업창, 다국어 작업 등에서는 오히려 추가적인 작업이 들어갈 수 있는 우려가 있다 ....

### import file
콘텐츠 파일의 상단과 하단에 `header`와 `footer`를 import하는 방식으로 사용한다. 신규 작업자나 개발자가 구조 파악하기도 쉬우며, 유지보수에도 편리하다.

## 결론
현재 대다수의 작업 특성상 `load content`방식을 오히려 손이 더 많이 갈 수 있기 때문에 `import file`방식으로 진행하고자 한다.

현재, webpack처럼 build가 가능한지 확인 중..