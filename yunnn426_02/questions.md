## 1. export named / default의 차이

![alt text](image-1.png)

<ol>
<li>
named export (유명 내보내기)
<ul>
<li>모듈 내에서 여러 개 존재 가능</li>
<li>import할 때는 export할 때와 동일한 이름을 사용한다.</li>
<li>구조분해할당(<code>{}</code>)을 사용해 가져온다.</li>
</ul>
</li>
<br/>
<li>
default export (기본 내보내기)
</li>
<ul>
<li>모듈 당 하나만 존재 가능</li>
<li>import할 때 원하는 이름 지정 가능</li>
<li>중괄호 없이 가져온다.</li>
</ul>
</ol>

## 2. 콜백 함수?
> 어떤 함수의 인자로 전달되는 함수

- 순차적으로 실행할 때 사용한다.

```js
function doSomething() {
    console.log(1)
}

function callMe(func) {
    func()
    console.log(2)
}

callMe(doSomething)
```
