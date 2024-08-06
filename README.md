Sass = css의 전처리기.<br>
Sass의 장점 → css보다 훨씬 간단한 표기법으로 css를 구조화하여 표현 가능, 가독성이 좋으며 재사용성을 높여주기 때문에 유지보수가 쉬움.<br>
Sass의 단점 → node 버전을 변경할 때 자주 다시 컴파일해야 함.<br>
Sass 설치 → node.js 설치 후 cmd 창에 node-v 입력(버전확인) + npm install sass -g 입력해서 다운로드 진행, 설치 확인 명령어는 sass --version(삭제 명령어는 npm uninstall node-sass)<br>
Sass 컴파일 → style.sass파일 작성 후 terminal 창(new terminal=ctrl+shift+`) 켜서 변환 구문 입력 → sass --watch sass/style.sass css/style.css (scss도 sass부분만 변경하면 동일)<br>
map 파일 → sass에서 지저분하게 코딩하더라도 css에서는 자동 정리가 되어 표시됨. 라이브서버 개발자모드에서는 css가 아닌 sass에서 몇 번째 줄(오류)인지 알려줌.<br>
<br>
<br>
📍무조건 style.sass가 마스터 파일이 되어야 함(컴파일 했기 때문). 독립적인 UI컴포넌트별로 외부 파일을 만들어서 마스터 파일에 삽입하는 식으로 불러올 수 있음. → @import "reset";<br>
<br>
nesting : html 구조와 동일하게 css코드도 들여쓰기를 사용해서 컴포넌트별로 css 구문을 구조화 시킴. ex) 호버를 걸고 싶을 땐 태그 안에 &:hover{}<br>
변수 : $bgBody: #eee; body {background: $bgBody;} → 유지보수가 쉬움.<br>
📁sass_mixin : 자주 만드는 UI컴포넌트가 있을 때, 해당 기능을 빠르게 만들어주는 코드의 CSS꾸러미를 패키징하는 기술. 믹스인 형태로 만들어 놓은 다음에 호출해주고 바꾸고 싶은 부분만 지정해주면 편하게 어떤 컴포넌트든 재사용 가능. ex) @mixin button ($wid:100px, $bg:gray){display, width, color 등}<br>
📁sass_for : <br>
📁sass_each : <br>
📁sass_each : <br>
