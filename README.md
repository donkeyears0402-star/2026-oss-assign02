# Assignment 02 - HTML & CSS Practice

**학번:** 21901037  
**이름:** 이준형 (Junhyung Lee)

## Assignment 02 수행 내용

W3Schools CSS Demo를 참고하여 동일한 HTML 구조에 서로 다른 CSS 스타일을 적용하는 웹페이지를 제작했습니다.

- **STEP 1:** `nostyle.html` — CSS 없이 HTML 구조만 작성
- **STEP 2:** `style1.html`, `style2.html` — W3Schools Stylesheet 1, 2 적용
- **STEP 3:** 브라우저 및 DevTools로 HTML/CSS 비교 확인
- **STEP 4:** Bootstrap Example — 미수행
- **STEP 5:** `index.html`에서 모든 페이지 연결, 각 페이지에 Home 링크 추가

## 페이지 설명

| 페이지 | 설명 | 파일 |
|--------|------|------|
| Index | 과제 메인 페이지, 전체 링크 모음 | [index.html](./index.html) |
| No Style | CSS 없는 기본 HTML 페이지 | [nostyle.html](./nostyle.html) |
| Style 1 | 초록 헤더 + 왼쪽 메뉴 + 오른쪽 사이드바 (W3Schools Style 1) | [style1.html](./style1.html) |
| Style 2 | 빨간 배경 + 둥근 버튼 메뉴 (W3Schools Style 2) | [style2.html](./style2.html) |

## URL

### GitHub Repository

https://github.com/2026-2-OSS/assign02-c01-21901037

### Vercel Deploy URL

> 배포 후 아래 URL을 실제 Vercel 주소로 수정하세요.

- https://assign02-c01-21901037.vercel.app/index.html
- https://assign02-c01-21901037.vercel.app/nostyle.html
- https://assign02-c01-21901037.vercel.app/style1.html
- https://assign02-c01-21901037.vercel.app/style2.html

---

## Weekly Review – Week 2

### Key Learning

1. HTML은 **구조**(제목, 문단, 목록, 링크)를 담당하고, CSS는 **디자인**(색상, 배치, 글꼴)을 담당한다.
2. `float`, `margin`, `position: absolute` 같은 CSS 속성으로 3단 레이아웃(메뉴·본문·사이드바)을 만들 수 있다.
3. 동일한 HTML에 다른 CSS를 적용하면 완전히 다른 화면을 만들 수 있다.

### HTML vs CSS

- **HTML:** 웹페이지의 뼈대. `div`, `h1`, `p`, `ul`, `a` 등으로 "무엇이 어디에 있는지" 정의한다.
- **CSS:** HTML 요소의 모양과 배치. `color`, `background-color`, `padding`, `float` 등으로 "어떻게 보일지" 정한다.

### Bootstrap 사용법

이번 과제에서는 Bootstrap Example(STEP 4)을 수행하지 않았다. Bootstrap은 미리 만들어진 CSS/JS 컴포넌트를 CDN으로 불러와 빠르게 반응형 웹페이지를 만들 때 사용한다.

### Problem & Solution

**문제:** 메뉴 항목에 `<a>` 태그를 사용했더니 링크 기본 밑줄이 표시되었다.

**해결:** `.menuitem a { text-decoration: none; }`를 추가하여 메뉴 링크의 밑줄을 제거했다. DevTools로 `<a>` 태그에 적용된 기본 스타일을 확인한 뒤 수정했다.

### AI Usage

- W3Schools CSS Demo 구조와 스타일을 맞추는 데 AI(Cursor)를 활용했다.
- AI가 생성한 CSS는 브라우저에서 직접 열어 W3Schools 원본과 비교하고, `grid` 등 어려운 속성은 `float`/`margin`으로 단순화했다.
- 메뉴 밑줄 문제, HTML 뼈대 통일, 주석 추가 등은 AI 제안을 확인 후 직접 검토하여 반영했다.

### Reflection

CSS에서 `float`와 `position: absolute`를 함께 쓰면 레이아웃이 어떻게 잡히는지 처음에는 헷갈렸지만, DevTools로 각 요소의 box model을 보면서 이해할 수 있었다. Bootstrap도 다음에 직접 적용해 보면 좋겠다.
