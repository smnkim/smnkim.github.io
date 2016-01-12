---
layout: post
title: "first-article"
subtitle: "jekyll first contents"
date: 2016-01-12 18:32:00
author: "smnkim"
header-img: "img/post-bg-06.jpg"
---

# MAC OS에서 *Jekyll* 설치하기


### 설치
~~~
$ xcode-select --install
$ \curl -sSL [https://get.rvm.io](https://get.rvm.io,"루비받기") | bash -s stable
$ source ~/.rvm/scripts/rvm
$ rvm install 2.2.0
$ gem install jekyll // 안되면 sudo gem install -n /usr/local/bin jekyll
~~~


### 지킬 프로젝트 설치
~~~
$ jekyll new 깃사용자명.github.io
~~~


### 로컬 확인
~~~
$ jekyll serve
~~~


### 깃 저장소와의 연동
~~~
$ git init
$ git remote add origin 저장소 URL
$ git add .
$ git commit -m "commit comment"
$ git push origin master
~~~


### 변경 후에 적용
~~~
$ git add . -A && git commit -m "commit comment"
$ git push -u origin master
~~~


### 추천 사이트

* [지킬 한글 문서](http://jekyllrb-ko.github.io/)
* [지킬 초보용 블로그](https://vjinn.github.io/about/)
* [프론트엔드](http://webberstudy.com)
