# Mon 19

## 배운 부분

- git에서 merge하는 방법, github에서 full request하는 방법
- API란? <br/>
  예시를 아주 잘 든 글을 봤다. [사이트 바로가기](http://blog.wishket.com/api%EB%9E%80-%EC%89%BD%EA%B2%8C-%EC%84%A4%EB%AA%85-%EA%B7%B8%EB%A6%B0%ED%81%B4%EB%9D%BC%EC%9D%B4%EC%96%B8%ED%8A%B8/)
  > API는 점원과 같은 역할을 합니다.<br/>
  > API는 손님(프로그램)이 주문할 수 있게 메뉴(명령 목록)를 정리하고, 주문(명령)을 받으면 요리사(응용프로그램)와 상호작용하여 요청된 메뉴(명령에 대한 값)를 전달합니다.<br/>
  > 쉽게 말해, API는 프로그램들이 서로 상호작용하는 것을 도와주는 매개체로 볼 수 있습니다.

* `window.screen.width`: 모니터 너비. 바뀌지 않음
* `window.outerHeight`: 브라우저의 높이(탭 포함).
* `window.innerHeight`: 브라우저의 높이(탭 불포함, 스크롤 포함)
* `document.documentElement.clientWidth`: 문서의 사이즈(스크롤바 불포함)

## 하루 돌아보기

공부에 정말 많은 시간을 보냈는데 얻은 것은 굉장히 적다. 이렇게 매일 공부하면 일주일 내에 번아웃이 오지 않을까. 뽀모도로와 비슷한 형식으로 `45분 공부 15분 휴식`을 취하고 있지만 한 번 집중하면 오래 공부를 하고 그에 대한 여파로 오래 쉬고 있다. 저 틀을 유지하는 것이 정말 중요하다.
<br/>
컴퓨터와 로컬저장소, 원격저장소 간의 add, commit, push... 참 헷갈린다. 게다가 소스트리에서 push하면 계속 403error가 나는데 골 때린다. 어쩔 수 없이 git에서 push하는데 차라리 git이 더 쉽다ㅋㅋ terminal이 더 쉽다니. ~~천상 개발자인가?(망언)~~

# Tue 20

## 배운점

- github fork하는 방법. 소스트리와 git에서 원격저장소로 push할 때 계속 에러가 난다... 아직 해결 못했지만 그로인해 배운 것이 많다.
  - push 에러를 해결하기 위해 구글링 했지만 제대로 얻는게 없다.
    - 원인을 깊게 생각하자. 말로 설명할정도로
    - 영어가 안된다면 굳이 읽지 말고 번역을 이용하자. 시간이 너무 오래 걸린다.
    - 영양가 없는 구글링은 그만. 해결이 안되면 잠시 내려두자. (머리 아파서 드러 누웠다)
  - ~~제대로 기록만 하면 별것도 아닌~~ 비밀번호 문제로 계속 막힌다. 비밀번호를 기록하고 백업하자. 내 기억력 믿을 수 없다.
  - 중고등 학생 때 답안지를 보며 수학문제 푸는 습관으로 현재 너무 힘들다. 강의와 책을 보면 답이 나와 있지만 이렇게해선 실력이 늘지 않아!! 생각을 깊게 하는 습관을 들여야 한다.
- 아이디 뒤에 `+`붙이면 계정을 여러개 만들 수 있다는 사실!! ~~(이걸로 카카페 계정 여러개 만들면!!)~~

## 하루 돌아보기

- `45분 공부 15분 휴식` 실천하지 못했다. 45분도 머리아프다. `25분 공부 5분 휴식`으로 해야겠다. 대신 철저하게 지키기!
- 너무 예민하면 주변에서 말을 시킬 수 없는 아우라를 뿜어낸다. 만약 말을 걸면 가자미 눈으로 처다본다... 고치자. 이렇게 일하면 도태 당해... 말을 걸기 편안한 상태를 유지해야 나에게도 남에게도 좋다. 결론은 `25분 공부 5분 휴식`
- 개발자는 의대에 준하는 준비기간이 필요하다는 [트윗](https://twitter.com/golbin/status/1384454871856803843?s=21)을 봤다. 난 시작한지 1년도 되지 않았다. ~~응애~~ 더 노력하자!

# Wed 21

## 배운점

- `Element.getBoundingClientReact()`: 모든 요소는 Element관련 API를 가져올 수 있다.
  - left : element의 왼쪽 위 x좌표
  - top: element의 왼쪽 위 y좌표
  - botoom: element의 오른쪽 아래의 y좌표
  - right: element의 오른쪽 아래의 x좌표
- `Client x,y`: 윈도우 브라우저 좌표(스크롤 불포함)<br/>
  `Page x,y`: 페이지의 좌표(스크롤 포함)<br/>
- `addEventListener`의 함수 전달 argument에는 항상 event라는 오브젝트를 전달한다.
- 네이밍 규칙 : css는 snake case(언더바(`_`) 이용, js는 camel case 이용
- 리로드 관련 이벤트
  - `DOMContentLoaded`: html이 다운 되었을 때 이벤트 발생<br/>
    (`defer 스크립트`는 html의 DOM이 준비된 후 js파일을 실행한다. 병렬적으로 스크립트를 다운로드 하지만 실행은 html에 추가한 순으로 진행된다. 따라서 실행순서가 중요한 경우 이용된다. `DOMContentLoaded`보다 빨리 실행된다. <br/>
    `async 스크립트`는 다운로드 된 순서대로 실행하기 때문에 스크립트 실행순서가 중요하지 않은 경우 이용한다.
    `<body>` 가장 아래 스크립트를 쓰면 HTML문서 다운로드 이후 스크립트가 실행되기 때문에 페이지가 느려질 수 있다. [추가설명 - javascript.info](https://ko.javascript.info/script-async-defer))
  - `load`: css, image, font 등 모든 이벤트가 다운 되었을 때
  - `beforeunload`: 페이지를 떠날 때
  - `unload`: `beforeunload` 뒤에 나옴

## 하루 돌아보기

- 인간이 살기 위해 해야하는 기본적인 행위, 밥 먹기, 잠자기, 요리하기, 산책하기, 💩하기 등을 굉장히 시간 아까워하고 항상 대충대충 넘기고 싶어했다. 하지만 이렇게 몰아치는 생활을 하니 깨달은 것이 있다. 이렇게 소소한 일들을 확실하게 해냈을 때 안정적이고 긍정적으로 하루를 보낼 수 있다는 것. 밥 대충 먹지 말고 소소함은 절대 소중한 것으로 뒷전에 밀리면 정신적으로 괴로워 진다는 것. 친구와의 대화는 너무 소중하다. 친구가 그리는 미래에 내가 있다는 것에 정말 감사한다. 결론은 **소소한 것을 지키자!**
- 오늘은 전반적으로 뽀모도로(`25분 공부 5분 휴식`)을 매우 잘 지켰다. 덕분에 오래 공부할 수 있었고 스트레스도 받지 않았다. **공부만큼 중요한 것은 휴식!**

# Thu 22

## 배운점

- 브라우저가 사용자에게 웹을 보여주기까지 어떤 과정을 거치는지 배움. <br/>
  html 파일 요청 > 파일 로딩 > dom으로 변환 > Rendering Tree > 요소 위치 배치 > painting
- 최대한 요소를 적게, 작게 만들어야 rendering tree를 빠르게 만들 수 있다.
- 사용자가 애니메이션을 쓸 때 layout 자주 일어나지 않게 해 브라우저 성능을 높인다. [참고 블로그](https://mygumi.tistory.com/238)
- 리팩토링하며 배운 것
  - css, image 등 함수보다 리소스를 먼저 불러와야 하는 경우 `addEventListener('load', function())`를 이용하는 것이 좋다
  - command shift p: 개발툴 팔레트 (layout 확인)
  - 사용자가 버벅임을 느끼지 않기 위해서 애니메이션이 16.67ms 안에 이뤄져야 함.

## 하루 돌아보기

브라우저 성능 개선 강의를 듣고 기존에 만든 간단한 좌표찾기 파일을 리팩토링 해봤다. (내가 생각해도 잘했다!!) 개발툴에서 이것저것 건들여 보다 `Rendering`에서 `paint flash`라는 체크박스에 체크했는데 초록색 레이저(?) 같은 광선이 마우스가 움직일 때마다 따라와 멋있었음. 브라우저 성능 개선으로 `Layout Shift Regions`가 보이지 않도록 했다. 리팩토링을 마치고 해당 강의를 보니 완전히 흡수한 느낌을 받았다. 정답을 보는 습관 대신 이렇게 스스로 해보려고 아등바등하는 모습, 칭찬해👏. (사실 재밌으니까 개발툴을 이것저것 건들였지 답이 안보이면 또다시 해설 강의부터 보려 했을거다. 운이 좋은 케이스일 수도... 경험이 쌓여야 제대로 판단할 수 있을거 같다.)

# Fri 23

## 배운점

- shopping list 웹을 static하게 만듬. 내일은 자바스크립트로 동적인 요소를 추가할 예정
- [드림코딩 아카데미](https://academy.dream-coding.com/)를 운영하시는 Ellie님의 유튜브 채널에서 T경력관리에 대한 [영상](https://youtu.be/ly7UabPJNvs)을 보며 (비전공자인 내게) 토양에 해당하는 자료구조와 알고리즘에 대한 지식이 전혀 없음을 깨달았다. 어려운 책을 보면 이해하기 힘들거 같아 일단 [엔지니어대한민국](https://www.youtube.com/user/damazzang) 유튜브 채널에서 공부하기로 함.

## 하루돌아보기

- 어제 낮잠을 자는 바람에 잠이 오지 않아 새벽에 잠들었고 덕분에 정오를 넘기기 전에 간신히 일어났다... 낮잠은 30분 이상을 넘기지 말자. 다음날 할 일을 제대로 하지 못한다.
- shopping list의 메인 색은 `chartreuse`다. 개발툴 `Rendering` - `Paint flashing`에서 pint가 일어날 때마다 이 색이 보이는데 너무 이뻐서 메인색으로 정했는데 역시 까리하다. 아주 맘에 들어

# Sat 24

## 배운점

- 주석 사용 방법. 어떻게 동작하는지가 아니라 왜 이렇게 작성했는지에 대해 쓰기.
- 유튜브 채널 `엔지니어대한민국`님의 영상을 보며 `Linked-List` 개념에 대해 배워 [내깃헙저장소](https://github.com/sibiwol/TIL/blob/main/lecture/Y_engineer-Korea/linked-list.md)에 정리했다. 내가 배우고 있는 언어인 javascript에서 배열 관련 매서드는 많이 보았지만 `linked-List`는 생소하여 [찾아보니](https://boycoding.tistory.com/33)변수 선언, `.append()` 등이 있었다.

## 하루 돌아보기

`나만의 규칙`으로 주말은 1. `TIL과 블로그 정리`하기! 2. `개발 외의 책 보기` 인데 주중에 끝내기로 했던 shopping list 웹을 마치지 못해 토요일이지만 강의를 봤다.(자료구조 공부처럼 `토양`에 해당하는 공부는 쉴 수 없다. 흙 없이 뿌리 내리는 것은 말이 안돼지. 아주 짧게, 그리고 길게 흙을 채우고 어느정도 채워지면 비료도 주자) 주중에 열심히 하고 주말에 휴식을 주자!!

# Sun 25

## 배운점

- `Linked-List` 단/양방향

## 하루 돌아보기

오늘 하루 동생과 카페에 가서 리프레쉬 제대로 했다. 한주를 시작할 힘을 얻었다! 하지만 주말에 하기로 한 블로그 글 쓰기를 하지 못해 아쉽다. 다음주도 있으니 자책말고 꾸준히 하자.

# WEEK 16, 한주 돌아보기

16주부터 다시 열심히 공부해서 취업에 성공하리라 (15주에) 결심했다. 한주를 돌아보니 만족스럽다. 간단한 `Shopping List`도 만들었다. (내 생각뿐이지만) 매우 감각적이라고 생각한다🤣🤣. (물론 이 프로젝트도 아쉬운 부분이 많다ㅠ 좀 더 배워 보완하고 싶다) 이렇게 달릴 수 있었던 이유는 뽀모도로 학습법과 아침마다 조금씩 읽고 있는 `프로그래머의 길, 멘토에게 묻다.` 책 덕분이라 생각한다. 아침마다 저자가 견습생(주니어)들에게 주는 조언을 들으며 조금씩 마음을 키웠다. <br/>

힘들었던 점은 배울 것이 너무 많다는 중압감. 이 세계는 정말 깊다. 깊기에 매력있지만 동시에 머리가 지끈거린다. 가장 큰 문제점은 내게 토양이 없다는 것. 하지만 여기에 중점을 둘 수 없어 일단 JavaScript 언어 배우기에 열중하고 아침엔 멘토와 같은 책을 읽고 저녁 자기 전엔 알고리즘과 자료구조에 대해 조금씩 배우기로 했다. 나의 목표는 아주 튼튼한 느티나무를 만드는 것이다!

# WEEK 17,다음주 계획

1. 조금 무리해서 `프론트엔드 필수 브라우저 101` 완강 또는, 해당 강의의 `리팩토링으로 배우는 코딩팁`까지 배우기
2. 현재 속도라면 `프로그래머의 길, 멘토에게 묻다.` 완독 가능. 그후`커리어 스킬`책을 읽을 예정
3. TIL 작성 전 (자기전) 유튜브 통해 Linked List 강의 꾸준히 1개씩 보기 + `그림으로 배우는 알고리즘`읽기(아직 주문 전이다.)
4. 블로그 글 1개 이상 작성하기.

17주차 한주 돌아보기에서 얼마나 지키는지 두고 보자고!!
