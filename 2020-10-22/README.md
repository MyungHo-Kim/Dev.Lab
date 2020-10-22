<h1>학습 결과</h1>
<ul>
    <li>Node.js의 가장 큰 특징은 바로 "Client가 아닌 Server 측에서 동작하는 Javascript"인 것이다.</li>
    <li>async: html 문서 다운로드 중간에 javascript 문서가 호출될 때 html 다운로드를 중지하지 않고 계속 받도록 한다. 이것은 DOMContentLoaded와 body 마지막에 javascript를 위치 시키는 것보다 좋은 효과를 낼 수 있다. 이 둘이 html이 모두 다운로드 될 때까지 javascript의 실행을 막고 있는것에 반면, async는 html의 로딩과는 관계없이 다운로드하고 바로 코드를 실행한다. 이때 이 자바스크립트가 html 요소와 관계된 처리를 한다면 문제가 발생할 수 있다. javascript에서 DOM 탐색 시 DOM이 아직 완전히 구현되지 않았을 수도 있기 때문이다. 그렇기 때문에 async는 해당 문서의 DOM이나 다른 자바스크립트의 파싱과는 관계없는 경우에 사용해야 한다.</li>
    <li>defer: async와는 다르게 defer로 지정된 문서의 순서대로 로딩하고 파싱한다. 서로 의존적인 경우 사용한다.</li>
</ul>

<h3>생각</h3>
<p>만약 자바스크립트가 HTML과 CSS 전에 실행되었다면 문제가 분명 발생할 것입니다. -> 어떠한 문제가 발생할 것인가? 문제의 구현은 가능한가?</p>

<h3>구현 자료</h3>
<ul>
    <li><a href="http://192.168.0.16:1114/Dev.Lab/2020-10-22/test.html" target="_blank">자바스크립트</a></li>
</ul>

<h3>참고 링크</h3>
<ul>
    <li><a href="http://webglsamples.org" target="_blank">Web GL 예제</a></li>
    <li><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs" target="_blank">Client-side web APIs</a></li>
</ul>