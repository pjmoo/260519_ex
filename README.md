# CSS 레이아웃 핵심(Flex & Position) & 부트스트랩/테일윈드 맛보기 📐

현대 웹 레이아웃 설계의 가장 핵심이 되는 요소 크기 계산법, 가로/세로 정렬 기법(Flexbox), 그리고 편리한 오픈소스 CSS 라이브러리(Bootstrap, Tailwind) 사용법을 익히는 실습 프로젝트입니다.

---

## 📂 학습 파일 구성 (Files)

- [01_box-sizing.html](file:///C:/workspace/260519_ex/01_box-sizing.html) : 테두리(border)와 여백(padding) 때문에 상자가 의도한 크기보다 커지는 문제를 방지하는 `box-sizing: border-box` 실습
- [02_block_inline.html](file:///C:/workspace/260519_ex/02_block_inline.html) : 줄을 혼자 다 쓰는 블록(Block) 요소와 다른 글자들과 한 줄에 배치되는 인라인(Inline) 요소의 차이점 파악
- [03_size-inheritance.html](file:///C:/workspace/260519_ex/03_size-inheritance.html) : 부모의 너비/높이를 비율(`%`)로 물려받는 자식 크기 상속 구조 실습
- [04_flex_position.html](file:///C:/workspace/260519_ex/04_flex_position.html) : 화면 특정 위치에 요소를 고정(position)하거나 정렬하는 기법 실습
- [05_flex.html](file:///C:/workspace/260519_ex/05_flex.html) : 현대적인 가로 정렬의 필수 도구인 Flexbox 정렬 기능 실습
- [06_bootstrap.html](file:///C:/workspace/260519_ex/06_bootstrap.html) : 미리 꾸며진 버튼, 상자, 네비게이션 등을 클래스명만 붙여 바로 쓰는 부트스트랩(Bootstrap) 사용 실습
- [07_tailwind.html](file:///C:/workspace/260519_ex/07_tailwind.html) : 별도의 CSS 파일 없이 HTML 태그 안에 유틸리티 클래스(예: `flex justify-center`)만으로 즉석 스타일링하는 테일윈드 CSS 사용 실습

---

## 🛠 배운 핵심 개념 (What We Learned)

- **Flexbox 정렬**: `display: flex;`를 부모 상자에 선언한 뒤, 가로 정렬(`justify-content`) 및 세로 정렬(`align-items`)을 손쉽게 수행하는 기법을 배웁니다.
- **Position 속성**: 화면에 요소를 둥둥 띄우거나(`absolute`), 브라우저 화면의 절대 좌표에 박아두는(`fixed`) 위치 결정 방식을 이해합니다.

---

## 🚀 실행 및 확인 방법 (How to Run)

1. 원하는 실습 파일을 브라우저로 엽니다.
2. 화면을 보면서 브라우저 개발자 도구(F12)의 '요소(Elements)' 탭을 켜서 Flex 정렬이나 박스 크기(margin, padding)가 어떻게 변하는지 분석합니다.

---

## PDF 기반 보충 정리

- Box Model의 실제 크기는 content, padding, border, margin의 관계로 결정된다. `box-sizing: border-box`를 적용하면 지정한 너비·높이에 padding과 border가 포함되어 레이아웃을 예측하기 쉽다.
- 블록 요소는 기본적으로 한 줄을 차지하고, 인라인 요소는 콘텐츠 크기만 차지한다. 필요에 따라 `display`를 바꾸되 문서 의미까지 바꾸지는 않는다.
- Flexbox는 부모에 `display: flex`를 선언한 뒤 주축은 `justify-content`, 교차축은 `align-items`로 정렬한다. `gap`은 항목 사이 간격을 일관되게 유지하는 데 유용하다.
- Bootstrap은 미리 준비된 컴포넌트와 규칙을 빠르게 적용하는 프레임워크이고, Tailwind CSS는 작은 유틸리티 클래스를 조합해 UI를 만드는 방식이다. 프로젝트의 디자인 자유도와 팀 규칙에 맞춰 선택한다.

## TIL

- 레이아웃이 어긋나면 `width`만 고치기 전에 box model과 부모의 flex 설정을 개발자 도구로 확인한다.
- 절대 위치 지정은 일반 문서 흐름에서 빠지므로, 정렬 문제의 기본 해법으로 남용하지 않는다.
