# 문서 구조를 위한 HTML5 시맨틱 태그

## `<header>` 태그 - 머리말 지정하기

사이트 전체의 헤더는 주로 페이지 맨 위쪽이나 왼쪽에 삽입하며 헤더의 내용으로는
주로 `<form>` 태그를 사용해 검색창을 넣거나
`<nav>` 태그를 사용해  사이트 메뉴를 넣음

`<header>` 태그는 본문 중에 사용해 해당 부분의 머리말로 사용할 수도 있음.

## `<nav>` 태그 - 문서를 연결하는 내비게이션 링크

`<nav>` 태그는 동일한 사이트 안의 문서나 다른 사이트의 문서로 연결하는 링크 모음을 나타냄.

내비게이션 메뉴뿐만 아니라 푸터에 있는 사이트 링크 모음 부분에도 많이 사용됨.
사용하는 위치의 영향을 받지 않아 `<header>`나 `<footer>` 태그 또는 `<aside>`태그 안에 포함시킬 수도 있고 독릭하여 사용할 수도 있음.
그리고 문서 안에 여러 개의 `<nav>` 태그를 사용할 경우 ID를 지정해 각 내비게이션에 맞는 CSS 를 지어줄 수 있음.

## `<section>` - 주제별 콘텐츠 영역 나타내기

문맥 흐름 중에서 콘텐츠를 주제별로 묶을 때 사용
그 안에는 섹션 제목을 나타내는 `<h1>~<h6>`이 사용됨.

또, `<section>` 태그 안에 `<section>` 태그를 넣을 수도 있음.

## `<article>` 콘텐츠 내용 넣기

`<section>` 태그와 비슷해 혼동하기 쉬운 `<article>` 태그는 

article의 사전적 의미가 신문이나 잡지의 기사를 뜻하는 것처럼 웹 상의 실제 내용을 넣음.

보통 블로그의 포스트나 태그를 적용한 부분을 떼어 내 독립적으로 배포하거나 재사용하더라도 완전히 하나의 콘텐츠가 된다면 `<article>` 태그를 쓰면 됨.

`<section>` 태그는 문맥 흐름 중에서 콘텐츠를 주제별로 묶을 때 사용
`<article>` 태그 안에 `<section>` 태그를 넣을 수도 있음

## `<aside>` - 본문 이외의 내용 표시

블로그에서 왼쪽이나 오른쪽 또는 하단에 사이드바가 이에 해당함.

사이드바는 필수 요소가 아니므로 광고나 링크 모음 등 문서의 메인 내용에 영향을 미치지 않는 내용들을 넣을 때만 사용

`<aside>` 태그는 본문 내용 외의 주변에 표시되는 기타 내용들을 나타냄.

## `<ifrmae>` - 외부 문서 삽입하기

일반적으로 웹 문서 안에 내용을 직접 입력하기도 하지만 다른 외부 문서를 삽입할 수도 있음.
이렇게 웹 문서 안에 다른 웹 문서를 가져와 표시하는 것을 **인라인 프레임(inline frame) 이라고 함.

즉, 인라인 프레임을 삽입하는 태그가 `<iframe>` 임.

**기본형** `<ifrmae src="삽입할 문서 주소" [속성="속성값"]></iframe>`

| 속성 | 설명 |
| width | 인라인 프레임의 너비 / 픽셀이나 백분율 값으로 표시 |
| height | 인라인 프레임의 높이 / 픽셀이나 백분율 값으로 표시 |
| name | 인라인 프레임의 이름 |
| src | 프레임에 표시할 문서의 주소 지정 |
| seamless | 프레임의 테두리를 없애 마치 본문의 일부처럼 보이도록 만들며 속성 값 없이 seamless라고 쓰면 됨(크롬, 사파리에만 지원) |

## `<footer>` - 제작 정보와 저작권 정보 표시하기

일반적으로 `<footer>` 태그 안에는 사이트 제작자의 연락처 정보와 저작권 정보를 표시

또한, `<footer>` 태그 안에는 `<header>`를 비롯해 `<section>, <article>` 등 다른 레이아웃 태그들을 모두 사용할 수 있음.

## `<address>` - 사이트 제작자 정보, 연락처 정보 나타내기

`<address>` 태그는 주로 `<footer>` 태그 안에 사용되는데 
웹 페이지 제작자의 이름이나 제작자의 웹 페이지 또는 피드백을 위한 연락처 정보를 넣는 데 사용됨.

## `<div>` 태그는 언제 사용할까?

HTML4에서 사용하던 `<div>` 태그는 사용할 수 없을까?

HTML5에서도 중요하게 사용됨.

HTML5에서는 주로 콘텐츠를 묶어 시각적 효과를 적용할 때 즉 콘텐츠에 CSS를 적용할 떄 `<div>` 태그를 사용함.

