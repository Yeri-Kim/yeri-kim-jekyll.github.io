---
layout: post
title:  "this"
date:   2019-05-03
categories: javascript
---

# this

JavaScript에서 복잡한 개념 중 하나는 `this` 키워드입니다.
`this` 는 모든 function의 scope 마다 정의되는 특별한 식별자(identifier) 입니다.

`this`는 해당 function이 소속된 object를 가르키고(refer) 있습니다.

this는 결국 객체라는 소리인데 이게 왜 복잡하다고 하지?

> 그 이유는 this를 사용하는 function이 어디에서 어떻게 호출되었느냐에 따라서 this가 가르키는 object가 다르기 때문입니다.

사실 this로 고생해보지 않은 사람은 this가 헷갈린다고 생각하지는 않을 것입니다.
설명을 들으면 다 이해가 가고, 개념도 어렵진 않기 때문입니다.
this로 고생하고, 하루 동안 원인모를 문제로 시달려봐야 '아~ this 란 복잡한거구나' 알게 됩니다.

다시 한 번 설명하자면 this는 코드를 작성할 때(함수가 정의 될 때) 정해지는 것이 아닙니다.
this가 가르키는 object는 해당 function을 어떻게 부르느냐, 어디에서 부르느냐에 따라 달라집니다.

```

```

In a method, this refers to the owner object.
Alone, this refers to the global object.
In a function, this refers to the global object.
In a function, in strict mode, this is undefined.
In an event, this refers to the element that received the event.
Methods like call(), and apply() can refer this to any object.







