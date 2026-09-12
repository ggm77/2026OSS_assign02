# OSS Assignment 02

- 학번: 22300378
- 이름: 서하민

## Assignment 02 수행 내용

HTML 문서의 기본 구조와 CSS의 역할을 이해하기 위해, 동일한 HTML 구조에 서로 다른 CSS 스타일을 적용해 보는 실습을 진행했습니다.

1. W3Schools CSS Demo(No StyleSheet Version)를 참고하여 `nostyle.html`을 제작했습니다.
2. W3Schools CSS Demo의 Stylesheet 1과 Stylesheet 3을 참고하여 `style1.html`, `style2.html`을 각각 제작했습니다.
3. 세 페이지를 브라우저와 DevTools로 비교하며, 동일한 HTML 구조가 CSS에 따라 어떻게 다르게 표현되는지 확인했습니다.
4. `index.html`을 만들어 모든 페이지로 이동할 수 있는 링크를 연결하고, 각 페이지에는 `index.html`로 돌아갈 수 있는 Home 링크를 추가했습니다.
5. 작업 단계별로 Git Commit을 진행하고 GitHub에 Push하여 Vercel을 통해 자동 배포되도록 했습니다.

## 페이지 설명 및 URL

| 페이지 | 설명 | URL |
| --- | --- | --- |
| `index.html` | 이번 과제에서 제작한 모든 페이지로 이동할 수 있는 메인 페이지 | https://2026-oss-assign02-jade.vercel.app/index.html |
| `nostyle.html` | CSS 적용 없이 HTML 구조만으로 작성한 기본 페이지 | https://2026-oss-assign02-jade.vercel.app/nostyle.html |
| `style1.html` | W3Schools CSS Demo의 Stylesheet 1을 참고하여 만든 페이지 | https://2026-oss-assign02-jade.vercel.app/style1.html |
| `style2.html` | W3Schools CSS Demo의 Stylesheet 3을 참고하여 만든 페이지 | https://2026-oss-assign02-jade.vercel.app/style2.html |

## Vercel Deploy URL

https://2026-oss-assign02-jade.vercel.app/index.html

## Weekly Review - Week 2

### Key Learning

1. HTML은 문서의 구조와 의미를, CSS는 그 구조를 화면에 어떻게 보여줄지를 담당한다는 것을 실습을 통해 직접 체감했습니다.
2. 동일한 HTML이라도 `display`, `margin`, `padding`, `border` 같은 속성을 조합하는 방식에 따라 전혀 다른 레이아웃이 나올 수 있다는 것을 배웠습니다.
3. `id`와 `class` 선택자를 활용해 특정 요소만 골라 스타일을 적용하는 CSS 선택자 사용법을 익혔습니다.

### HTML vs CSS

HTML은 제목, 문단, 목록, 링크 등 콘텐츠의 종류와 순서를 정의하는 뼈대이고, CSS는 그 뼈대에 색상, 여백, 배치 등 시각적인 스타일을 입히는 역할을 합니다. 즉 HTML이 "무엇을 보여줄지"를 정한다면, CSS는 "어떻게 보여줄지"를 정한다고 정리할 수 있습니다.

### Problem & Solution

`style1.html`을 만들 때 `main` 영역에 `nav`, `content`, `sidebar`를 가로로 나란히 배치하려 했으나 기본 `display` 값 때문에 요소들이 세로로 쌓이는 문제가 있었습니다. `main`에 `display: flex`를 적용하고 `nav`, `sidebar`의 너비를 `min-width`/`max-width`로 고정한 뒤에는 의도한 대로 가로 3단 레이아웃이 만들어졌고, DevTools의 레이아웃 패널로 각 요소의 박스 크기를 확인하며 문제를 해결했습니다.

### AI Usage

CSS 속성 조합이 W3Schools 예제와 시각적으로 얼마나 유사한지 검토하고, 레이아웃이 깨지는 원인을 분석하는 과정에서 AI(Claude Code)의 도움을 받았습니다. AI가 제안한 CSS 코드는 그대로 사용하지 않고, 브라우저에서 직접 렌더링 결과를 확인한 뒤 색상 값과 여백 수치를 원본 예제와 비교하며 수정했습니다.

### Reflection

같은 HTML 구조라도 CSS의 `display` 속성 값(`flex`, `flow-root` 등)에 따라 레이아웃 전체가 달라질 수 있다는 점이 새로웠습니다. 앞으로는 `flex`와 `grid` 외에 다른 레이아웃 관련 속성들도 더 찾아보고 싶습니다.
