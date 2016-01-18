---
layout: post
title: "git 이론 -1부"
subtitle: ""
date: 2016-01-18 19:25:00
author: "smnkim"
header-img: "img/smnkim.jpg"
---



## git이란
----

분산버전관리시스템으로써 속도와 효율성에서 아주 뛰어난 성능을 가지고 있다.

로걸에 DB를 가지고 있어 모든 작업을 로컬에서 할 수 있다.

로컬에서 대부분 작업을 수행하므로, 네트웍 비용이 거의 안들기 때문에 속도가 빠르고 비용이 절감된다.

서버에 문제가 발생한다고 하더라도, 로컬에 DB가 있기때문에 공유에는 차질이 생길지라도 작업은 계속 할 수 있다.

git은 SHA-1 40Byte HASH코드를 사용하는데, 파일의 내용을 바탕으로 Key가 생성된다.




----         

<br><br><br>

## Patch vs Snapshot

----
svn같은 경우, 버전 관리를 Patch를 통해서 진행한다.
개발기간이 길어질수록 Pacth에 대한 모든 기록을 불러와야 하기 떄문에 속도가 느려지는 단점이 있다.

<br>
Snapshot 같은 경우, 변경된 파일의 새로운 오브젝트를 가지고 있고 변경되지 않은 파일은 레퍼런스를 통해 주소값을 참조한다.
----


<br><br><br>

## 다양한 git 명령어

----

- git config --global
- git init
- git clone
- tree
- add
- commit
- etc.

----