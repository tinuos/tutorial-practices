# # MDN - HTML Assesement: Structuring a page of content

- [실습 페이지](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Structuring_a_page_of_content)

---
---

## 요구사항 분석

- 웹 페이지에 대한 구조잡기
  - 시맨틱 태그 활용
- 자료 제공 활용
  - 마크업할 HTML 코드
  - 이미지 파일
  - 스타일 시트

### 페이지 구조 잡기

- header
  - 사이트 로고, 네비게이션 메뉴
- main contents
  - 2개의 컬럼 포함
    - welcome text
    - sidebar(이미지 썸네일을 포함한)
- footer
  - 저작권 정보 및 credits

### Semantic tag 활용

콘텐츠 확인 후 각각의 구조에 따라 적절한 HTML 태그 사용(사이트 예제 이미지 참고)

![페이지 예제 이미지](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Structuring_a_page_of_content/example-page.png)

- header
- navigation menu
- main content
- welcome text
- image sidebar
- footer

### 제공된 스타일 시트 적용하기

- link 요소 활용

---

## 정리

- 모던 웹 페이지 구조를 직접 마크업해보는 실습
- header, nav, main, aside, footer 등을 사용

> 위에 언급한 큰 구조들의 기본적인 형태와 특히 네비게이션 바를 목록화하여 작성할 수 있는 방법에 대해 간단히 배울 수 있었다.

> aside가 main 안에서 분류되도록 조건을 명시하고 있는데, 가장 좋아하는 새들의 썸네일을 보여주는 기능이라 웹 페이지의 주요 내용과 관련 있어 main에 포함되는 것 같다. 만약 메인 콘텐츠와 관련없는 광고나 링크 모음일 경우 aside를 활용할 수 있겠지만 main 안에 배치하지 않고 영역을 따로 구분해볼 수 있겠다.

> Semantic tag들을 사용할 때 각기 다른 요소 간 계층적인 구조를 어떻게 잡을지 계획하는 것도 중요한 것 같다. 계층 간 관계를 명확히 해야 구조적인 의미 파악이 쉽고 또한 CSS로 레이아웃을 잡기에도 편할 것 같다.