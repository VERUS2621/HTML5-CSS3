# 웹에서 사용하는 멀티 미ㅣㄷ어

오디오나 비디오 같은 멀티미디어를 직접 재생할 수 없던 과거의 브라우저에서는
`플러그인(plug-in)` 프로그램을 사용함

그래서 예전에는 인터넷에서 음악을 듣거나 온라인 강의를 시청하려고 할 떄 특정 프로그램을 설치라하는 메세지가 뜨곤 하는데 그게 바로 플러그인임.

2020년 이후로 플래스 플레이어는 지원을 종료했음

현재는 플러그인 방식에서 벗어나 HTML5 비디오 표준으로 전환함에 따라, 동영상 재생은 더이상 플러그인에 의존하지 않고,
브라우저 자체에 지원한느 방식을 변함 

- > 성능과 보안이 크게 향상됨.

## `<object>` `<embed>`

### `<object>` - 외부 파일 삽입하기

웹 브라우저에서 직접 재생할 수 없는 자바 애플릿, PDF 파일, 플래시 무비 같은 콘텐츠를 웹 문서 안에 포함시키기 위해 사용함.
또한 다른 HTML 문서도 웹 문서에 포함시킬 수 있음.

**기본형**
`<object data="경로" type="유형" [name="이름" width="너비" height="높이"]></object>`

특정 외부 파일을 가져와 표시할 것인지 여부를 알려주기 위해 data 또는 type 둘 중 하나를 반드시 사용해야 함.

data : 외부 파일의 경로를 지정
type : 포함시킨 내용의 유형을 지정
name : 다른 요소들과 구분할 수 있는 이름 지정
width : 포함시킨 내용의 너비 값을 지정
height : 포함시킨 내용의 높이 값을 지정

## `<embed>` - 외부 파일 삽입하기

**기본형** `<embed src="경로" type="유형" width="너비" height="높이">

`<embed>` 태그는 주로 `<object>` 태그를 지원하지 않는 이전 브라우저에서 삽입

----

## 멀티미디어의 웹 표준화

HTML5는 PC뿐만 아니라 웹 브라우저가 설치되니 모든 기기에 적용되는 웹 표준이므로  플러그인 프로그램 없이 웹 브라우저 자체에서 멀티미디어를 재생할 수 있음.
웹에서 지원하는 비디오 / 오디오 파일에는 여러 종류가 있음.

| 종류 | 확장자 | 설명 |
| --- | --- | --- |
|  | mp4 | 고화질 영상을 지원해 많은 사이트에서 사용하고 있음. 라이선스가 있지만 웹에서 사용할 경우에는 무료로 사용할 수 있음 |
| 비디오 | webm | 화질이 우수하고 무료로 제공되어 최근 많이 사용되고 있음 |
| | ogv | 화질은 다른 비디오 유형보다 떨어지지만 무료라는 장점 떄문에 webm 형식이 등장하기 전에 많이 사용했음 |
| 오디오 | mp3 | 대부분의 음원에서 사용되지만 라이선스 때문에 유료로 사용해야 함. |
| | ogg | 무료이므로 게임 등에서 많이 사용함 |

|               | **MP4 (H.264)** | **WebM (VP8/VP9)** | **Ogv (Theora)** | **MP3**      | **Ogg (Vorbis)** |
|---------------|-----------------|--------------------|------------------|-------------|------------------|
| **Chrome**    | O (v3.0+)        | O (v6.0+)           | O (v3.0+)         | O (v26.0+)  | O (v6.0+)         |
| **Firefox**   | O (v21.0+)       | O (v4.0+)           | O (v3.5+)         | O (v21.0+)  | O (v3.5+)         |
| **Safari**    | O (v3.0+)        | X                   | X                 | O (v6.0+)   | X                |
| **Edge**      | O (v12.0+)       | O (v14.0+)          | X                 | O (v12.0+)  | O (v15.0+)        |
| **Opera**     | O (v10.5+)       | O (v10.6+)          | O (v10.5+)        | O (v15.0+)  | O (v10.6+)        |
| **Android**   | O (v3.0+)        | O (v4.0+)           | O (v3.0+)         | O (v3.0+)   | O (v4.0+)         |
| **iOS Safari**| O (v3.1+)        | X                   | X                 | O (v3.1+)   | X                |

확장자옆 괄호()는 코덱을 의미함.

### HTML5와 비디오 코덱

원본 비디오를 최대한 압축해 컴퓨터에서 사용할 수 있는 비디오 파일로 변환해야 함.

이를 `인코딩(encoding)` 이라고 함.

반대로 비디오 파일에 저장되어 있는 비디어 정보를 가져와 비디오 플레이어에 보여 주는 과정을 디코딩(decoding) 이라고 함.

**인코딩과 디코딩을 수행하는 것이 비디오 코덱**임

HTML5에서는 플러그인 프로그램 없이 브라우저에서 직접 재생할 수 있는 비디오 코덱만 허용하는데 아직 한 가지 코덱으로 통일되지 않아 여러 코덱이 사용되고 있음.


