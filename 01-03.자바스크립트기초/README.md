# JavaScript란?
**객체기반의 스크립트 프로그래밍언어**이다.<br/>
동적이며, 개발자가 **별도의 컴파일 작업을 수행하지않는 인터프리터언어**이다.

# JavaScript 실행순서
위에서 아래로 진행

# JavaScript 장단점
장점<br/>
html안에서 script태그로 코드를 바로 작성하므로 **개발이빠르고, 컴파일작업을 수행하지않기때문에 즉시 실행이 가능하다.**

단점<br/>
**브라우저**는 악성웹페이지가 개인정보에 접근하거나 사용자의 데이터를 손상하는 것을 막기위한 목적으로 **보안을위해 자바스크립트의 기능에 제약을 걸어놓았다.** <br/>
웹브라우저에서 실행되기때문에 일부 보안상의 제약이 있으며, 브라우저에서 웹페이지를 열때 안정하고 위험에처하지않도록 보장해야한다. <br/>
os에 직접 접근할수없고, 하드디스크를읽고쓰거나 다른프로그램을 호출할수없다.

# JavaScript 표준
자바스크립트의 표준은 ECMAScript으로,  Ecma 인터내셔널에 의해 제정된 ECMA-262 기술 규격에 의해 정의된 범용 스크립트 언어이다.

# JavaScript의 성장
초창기 JavaScript는 단지 브라우저를 제어하기 위한 언어였다. 하지만 점차 웹은 단순히 정보를 제공하는것에 그치지않고 서로 교류를 하는 방향으로 바뀌어가고있다.

## 1. AJAX
자바스크립트의 라이브러리 중 하나. **비동기방식**으로 데이터를 교환할수있는 통신기능이다.<br/>
이전의 웹페이지는 html로 시작해 html로 끝나는 코드를 서버로부터 전송받아 웹페이지 전체를 렌더링하는 방식으로 동작했었는데,<br/>
AJAX는 전체페이지를 새로고치지않고도 **페이지의 일부만을 위한 데이터를 로드하는 기법**이다.<br/>
따라서 웹페이지의 속도가 향상되었지만 히스토리관리가 안되는 문제점이있다.<br/>

## 2. DOM
DOM은 **html문서에 대한 인터페이스**다.<br/>
따라서 여러프로그램들이 페이지의 콘텐츠및구조,스타일을읽고 조작할수있도록 API를 제공한다.<br/>
DOM의 구조는 "노드트리(Node Tree)" 로표현된다.
<img src="https://velog.velcdn.com/images%2F5o_hyun%2Fpost%2F9119802b-72a6-4ead-a306-0d09cc6552ba%2F1111.png">

DOM은 html과 비슷해보이지만 다르다.<br/>
- 자바스크립트에 의해 수정될수있는 동적모델이다.<br/>
- 가상요소를 포함하지않는다 (::after)<br/>
- 보이지않는 요소를 포함한다. (display:none;)<br/>

## 3. jQuery
jQuery는 이벤트처리, ajax의 상호작용 및 애니메이션을 수행하는 자바스크립트의 라이브러리로, 단순화하여 설계되었다.<br/>
DOM을 더욱 쉽게 조작할수있게되었고, ui관련기능을 최소한의 코드로 짤수있다.

## 4. V8 자바스크립트엔진
원래 자바스크립트는 브라우저에서만 실행됬었는데, V8엔진을 기반으로 자바스크립트를 브라우저가 아닌 다른 운영체제에서도 사용할 수 있게되었다.

## 5. Node.js
Node.js는 자바스크립트를 실행할수있는 런타임환경이다.(실행기임)<br/>
Node.js를 실행하면 자바스크립트를 컴파일하여 실행할수있고, 이를 활용해 자바스크립트로 된 서버, 랩, 소프트웨어를 만들 수 있다.

## 6. SPA 프레임워크
대표적으로 Vue.js, React, Angular가 있다.<br/>
서버-클라이언트간의 상호작용이 많아지면서 복잡한 개발규모가 커지고 이에따라 프레임워크가 등장했다. <br/>
대표적으로 기업에서 많이 사용하는 React도 결국 브라우저 위에서 돌아가는 Javascript일 뿐이며 다만 node.js 환경에서 작성하고, 실행해보고, 작은 용량으로 압축해서 브라우저위에서 돌아가는 프론트 프레임워크(라이브러리)이다.

> 왜 계속 발전하고 변화할까? <br/> 시간이지나면서 인터넷이용자, 네트워크속도 등이 중요해지면서 브라우저가 감당해야할 자바스크립트의 양이 많아지면서, <br/>많은잉의 자바스크립트를 읽고 실행하기 위해 브라우저 엔진의 개선이 지속적으로 필요한것이다.

# ES6 브라우저 지원 현황
왠만한 브라우저에서 지원이되지만 간혹 ie나 구형브라우저에서 지원이 안된다.<br/>
can i use에서 찾아보고, 바벨등을 이용해 다운그레이드 해줄 필요가있다.
