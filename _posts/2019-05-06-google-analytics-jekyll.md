---
layout: post
title:  "Jekyll에 Google Analytics 붙이기"
date:   2019-05-06
categories: jekyll
---

요즘 우리 wecoders! 1일 1포스팅에 열정적인데 :heart_eyes: 아마 본인 블로그가 검색이 되는지?
된다면 얼마나 들어오는지 궁금하실 것 같아요.

Google Analytics(이하 GA)를 추가해서 알아보도록 하겠습니다.

### google-analytics.html 파일 가져오기

GA를 추가하려고 봤더니 `_includes/google-analytics.html` 이라는 파일이 있더라구요.
아마도 쓰는 사람이 많아서 추가하기 좋게 미리 세팅되어있는 것 같습니다.

다시 한 번 minima 테마 위치를 찾아서
```
bundle show minima
```
_includes 디렉토리 밑에 있는 google-analytics.html을 내 블로그의 _includes 밑에 넣어줍니다.

### GA 가입하기

[GA 홈](https://analytics.google.com)에서 Sign Up을 누르고 아래와 같이 세팅했습니다.
<img src="/img/190506-ga.png" width="340" />

가입하자마자 첫 화면에 Tracking ID가 나올거예요.

