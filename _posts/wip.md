---
layout: post
title:  "React 2 - Component와 Props"
date:   2019-04-17
categories: react
---

[React 공식문서](https://reactjs.org/docs/components-and-props.html)를 참고하여 번역하고 내용을 추가하였습니다.

## Component
프론트앤드 개발을 하면 Component 라는 단어를 참 많이 씁니다.
component(컴포넌트)란 재사용 가능한 UI 단위라고 생각하시면 됩니다.


Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. You can find a detailed component API reference here.

Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

React lets you define components as classes or functions. Components defined as classes currently provide more features which are described in detail on this page. To define a React component class, you need to extend React.Component:

class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
The only method you must define in a React.Component subclass is called render(). All the other methods described on this page are optional.


#### reference
* react docs