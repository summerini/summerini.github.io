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
<br><br><br>

## 🦥 파일 디렉토리 조작 명령어
* cp
  - 파일 및 디렉토리를 복사하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ cp b.txt b2.txt  
    [vagrant@host1 bitcamp-ncp]$ ls  
    b2.txt  b.txt  c.txt  d.txt  hello2.txt  README.md  x.txt  
<br>

* mkdir
  - 디렉토리를 만드는 명령어  
* mv
  - 파일 및 디렉토리를 이동하고 이름을 변경하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ mkdir test  
    [vagrant@host1 bitcamp-ncp]$ ls  
    b.txt  c.txt  d.txt  gitcamp-ncp2  hello2.txt  README.md  test  x.txt  
    [vagrant@host1 bitcamp-ncp]$ mv b2.txt test  
    mv: cannot stat ‘b2.txt’: No such file or directory  
    [vagrant@host1 bitcamp-ncp]$ mv x.txt test  
    [vagrant@host1 bitcamp-ncp]$ ls  
    b.txt  c.txt  d.txt  gitcamp-ncp2  hello2.txt  README.md  test  
    [vagrant@host1 bitcamp-ncp]$ cd test  
    [vagrant@host1 test]$ ls  
    x.txt  
    [vagrant@host1 test]$  
<br>

* rm
  - 파일 및 디렉토리를 삭제하는 명령어  
    [vagrant@host1 test]$ rm x.txt  
    [vagrant@host1 test]$ ls  
<br>

* ln
  - 하드 링크 또는 심볼릭 링크를 만드는 명령어  
    [vagrant@host1 bitcamp-ncp]$ ln -s /1.txt  
<br>
