# 여백을 조절하는 속성

![img](/CSS3/04/04-1/border_padding.png)

## margin 속성 - 요소 주변 여백 설정

**기본형** `margin-[top/right/bottom/left.]: <크기> | <백분율> | auto`

### margin overlap 현상

박스 모델의 마진 속성을 사용할 때는 주의해야할 것이 있음

그것은 바로 요소를 세로로 배치할 경우, 마진과 마진이 만날 때 마진 값이 큰 쪽으로 겹치는 것.
이런 현상을 **마진 중첩** 또는 **마진 상쇄**라고 함.

가로로 즉, 인라인 요소로 배치할 때는 마진 중첩, 마진 상쇄는 일어나지 않음

## padding 속성 - 콘텐츠 영역과 테두리 사이 여백 설정

`padding-[top/right/bottom/left.]: <크기> | <백분율> | auto`

