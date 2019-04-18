---
layout: post
title:  "React 2 - state"
date:   2019-04-17
categories: react
---

## JSX

```jsx
const hi = <p>Hi</p>;
```
위의 코드는 javascript인가요, html인가요? 네.. 둘 다 아닙니다. 확인해보고 싶으면 개발자도구 콘솔에 작성해보세요.

위의 문법은 JSX라고 불리는 JavaScript 확장버전입니다. *syntax extension for JavaScript*라고 합니다. HTML과 아주 비슷하게 생겼고 javascript 파일 내에서 작성할 수 있습니다.

JSX는 원래의 JavaScript 문법이 아니기 때문에, .js 파일내에 JSX 문법이 있으면 브라우저에서 해석하지 못합니다. 문법 오류가 납니다.

React.js를 사용하기 위해 JSX 문법이 포함되어 있으면, 해당 파일을 정규 javascript 문법으로 변환시키는 컴파일 과정이 필요합니다. 컴파일 방법과 환경은 offline 수업에서 다루도록 하겠습니다. 일단은 JSX Compiler가 깔려있는 에디터에서 연습을 해보도록 하겠습니다.

### JSX element
JSX는 .js 파일 어디에서나 사용할 수 있습니다. 변수에 저장할 수도 있고, 함수의 인자로 넘길 수도 있습니다.

평소에 작성하던 HTML처럼 작성하시면 됩니다.
```jsx
const hi = <p>Hi</p>;

const myFavorite = {
    food: <li>샐러드</li>,
    animal: <li>dog</li>,
    hobby: <li>programming</li>
};
```

### JSX attribute

태그에 attribute(속성)을 주고 싶을 때는 항상 "" 쌍따옴표로 감싸주세요.
attribute를 추가하고 싶을 때는 실제 HTML에서 쓰는 속성명과 다를 수 있으니 [react 공식문서](https://reactjs.org/docs/dom-elements.html#all-supported-html-attributes)를 참고해주세요.

예를 들어, class를 주고 싶을 때 원래 속성명은 `class`이지만 JSX에서는 `className`을 사용해야 합니다.
```jsx
const hi = <input readOnly={true} />;

const myFavorite = {
    food: <li>샐러드</li>,
    animal: <li>dog</li>,
    hobby: <li className="list-item">programming</li>
};
```

#### [Self-Closing Tag](https://zhenyong.github.io/react/tips/self-closing-tag.html)
그리고 JSX에서는 self closing tag는 항상 가능합니다만, `<input>`과 같이 `/` 를 없이 쓰는 것은 불가능합니다.
태그가 끝날 때는 항상 `/` 으로 끝내주셔야 합니다.

`<div />`와 `<div></div>`는 같은 표현입니다.

#### Nested JSX

1. 소괄호로 감싸기
```jsx
const good = (
    <div>
        <p>hi</p>
    </div>
);
```
중첩된 요소를 만들려면 () 소괄호로 감싸주세요!

2. 항상 하나의 태그로 시작
```jsx
const wrong = (
    <p>list1</p>
    <p>list2</p>
);
```
위와 같이 제일 처음 요소가 sibling이면 안됩니다. 무조건  하나의 태그로 감싸져야 합니다.
아래의 코드처럼 첫 요소는 무조건 하나의 태그로 감싸주어야 합니다.
```jsx
const right = (
    <div>
        <p>list1</p>
        <p>list2</p>
    </div>
);
```

[codepen](https://codepen.io/anon/pen/oOqjdp) 에서 간단히 확인할 수 있습니다.

#### reference
* codecademy