---
layout: post
title: "프로젝트를 진행하면서"
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

- git config [--global]
    - 사용자 정보를 설정하는 단계
    - 글로벌 속성을 사용 할 경우, 홈 디렉토리에 .gitconfig가 저장되느냐, 개인 저장소에 저장되느냐의 차이가 있다.
    - 보통 프로젝트 단위로 진행 할 경우에는 개인 저장소에 config하는 것이 맞다.
    - config를 설정 한 후에, 보통 .gitignore파일에서 컴파일에 의해 자동으로 생성되는 파일에 대해 추적하지 않겠다는 것을 함께 설정해준다.
- git init
    - 프로젝트가 처음 시작될때 사용하는 명령어
- git clone
    - 기존에 있던 프로젝트를 가져올때 사용하는 명령어
- tree
    - tree .git을 할 경우, .git에 있는 디렉토리 구조를 볼 수 있다.
- add
- commit
- etc.

----

<br><br><br>

## Working directory, Index, Repository

----

새로 생성, 혹은 변경한 파일들은 Working directory에 보관되며 add명령을 하게 되면, Index라는 git의 중간 영역에 Staging된다.

add를 하고나서, add한 파일을 다시 수정 할 경우, 수정한 파일은 Working directory에 보관되며 추가로 add명령을 해야 수정된 파일이 Index영역에 보관된다.

commit명령을 하게 되면 Index영역에 Staging된 오브젝트 파일이 Local Repository에 보관된다.

push명령을 통해 Server Repository에 비로소 적용이 된다.

----


### 2부에서는 Remores와 Brance, Merge, Rebase, Git Flow에 대해 정리할 예정