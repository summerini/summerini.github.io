---
title: "[13일차] 파일 디렉토리 조작 명령어"
excerpt: "cp, mv, mkdir, rm, ln"

categories:
  - Categories2
tags:
  - [Linux]

permalink: /categories2/post-name-here-2/

toc: true
toc_sticky: true

date: 2022-11-23
last_modified_at: 2022-11-23
---

## 🦥 과제
* cp, mv, mkdir, rm, ln
* 파일 디렉토리 조작 명령어에 대한 설명과 사용 예시, 출력 결과 일부를 알아보자
<br>

## 파일 디렉토리 조작 명령어
<br>

* cp
  - 파일 및 디렉토리를 복사하는 명령어<p>
    [vagrant@host1 bitcamp-ncp]$ cp b.txt b2.txt<p>
    [vagrant@host1 bitcamp-ncp]$ ls<p>
    b2.txt  b.txt  c.txt  d.txt  hello2.txt  README.md  x.txt<p>
<br>

* mkdir
  - 디렉토리를 만드는 명령어<p>
* mv
  - 파일 및 디렉토리를 이동하고 이름을 변경하는 명령어<p>
    [vagrant@host1 bitcamp-ncp]$ mkdir test<p>
    [vagrant@host1 bitcamp-ncp]$ ls<p>
    b.txt  c.txt  d.txt  gitcamp-ncp2  hello2.txt  README.md  test  x.txt<p>
    [vagrant@host1 bitcamp-ncp]$ mv b2.txt test<p>
    mv: cannot stat ‘b2.txt’: No such file or directory<p>
    [vagrant@host1 bitcamp-ncp]$ mv x.txt test<p>
    [vagrant@host1 bitcamp-ncp]$ ls<p>
    b.txt  c.txt  d.txt  gitcamp-ncp2  hello2.txt  README.md  test<p>
    [vagrant@host1 bitcamp-ncp]$ cd test<p>
    [vagrant@host1 test]$ ls<p>
    x.txt<p>
    [vagrant@host1 test]$<p>
<br>

* rm
  - 파일 및 디렉토리를 삭제하는 명령어<p>
    [vagrant@host1 test]$ rm x.txt<p>
    [vagrant@host1 test]$ ls<p>
<br>

* ln
  - 하드 링크 또는 심볼릭 링크를 만드는 명령어<p>
    [vagrant@host1 bitcamp-ncp]$ ln -s /1.txt<p>
<br>
