---
title: "[13일차] 파일 시스템 탐색 기본 명령어"
excerpt: "pwd, cd, ls, file, less"

categories:
  - Categories2
tags:
  - [Linux]

permalink: /categories2/post-name-here-1/

toc: true
toc_sticky: true

date: 2022-11-23
last_modified_at: 2022-11-23
---

## 🦥 과제
* pwd, cd, ls, file, less
* 파일 시스템 탐색 기본 명령어에 대한 설명과 사용 예시, 출력 결과 일부를 알아보자
<br>

## 파일 시스템 탐색 기본 명령어
<br>

* pwd
  - 현재 작업중인 디렉토리를 표시하는 명령어 <p>
    [vagrant@host1 git]$ pwd <p>
    /home/vagrant/git
<br>
      
* cd
  - 디렉토리로 이동할 때 사용하는 명령어 <p>
    [vagrant@host1 ~]$ cd git <p>
    [vagrant@host1 git]$
<br>
      
* ls
  - 디렉토리 내용을 나열하는 명령어 <p>
    [vagrant@host1 git]$ ls <p>
    bitcamp-ncp  bitcamp-ncp2  bitcamp-study <p>
    [vagrant@host1 git]$ <p>
<br>
      
* file
  - 파일 타입을 확인하는 명령어 <p>
    [vagrant@host1 bitcamp-ncp]$ file b.txt <p>
    b.txt: ASCII text <p>
<br>

* less
  - 파일 내용을 표시하는 명령어 <p>
    [vagrant@host1 bitcamp-ncp]$ less b.txt <p>
    1111 <p>
    2222 <p>
    3333 <p>
    4444 <p>
    5555 <p>
    6666 <p>
    b.txt (END) <p>
<br>
