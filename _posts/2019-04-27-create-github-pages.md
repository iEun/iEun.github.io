---
layout: default
title:  "Github Pages 만들기"
---



이번 포스트는 **Github page**를 만드는 방법입니다.
>Github Pages는 Github repository로 바로 호스팅되는 정적인 호스팅 서비스입니다. Github free로 생성할 수 있지만 Github Pages Repository를 private으로 생성하고 싶으면 Github pro 계정을 사용해야한다고 하네요.
<br>

## 1. 새로운 repository 만들기

![스크린샷 2019-04-26 오전 11.36.34](https://i.imgur.com/8PV1EkY.png)

Github 에 접속하여 **Create a new repository** 를 선택합니다. 이름은 [username].github.io. 와 같이 생성합니다. <u>username이 일치하지 않는 경우에는 제대로 동작하지 않는다고 하니 꼭 일치하게 생성합니다.</u>

## 2. index.html 파일 생성하기
터미널을 이용해서 index.html파일을 생성해봅니다.

```
git clone https://github.com/username/username.github.io
```
터미널을 열고 아까 생성한 repository를 클론합니다.



```
cd username.github.io
echo "Hello World" > index.html
```
아래와 같이 Hello world 라는 Text를 가진 index.html을 생성해주고요.

## 3. repository에 commit하기
```
git add --all
git commit -m "Initial commit"
git push -u origin master
```
해당 repository에 커밋해줍니다.

## 4. Github page가 만들어졌는지 확인


![스크린샷 2019-04-26 오전 11.52.11](https://i.imgur.com/VRK9Cdp.png)

https://[username].github.io 에 접속하여 확인해보면 Hello World 라는 텍스트가 찍힌 Github page를 확인할 수 있습니다.
