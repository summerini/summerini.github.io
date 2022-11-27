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
<br><br><br>

## 🦥 파일 시스템 탐색 기본 명령어
* pwd
  - 현재 작업중인 디렉토리를 표시하는 명령어  
    [vagrant@host1 git]$ pwd  
    /home/vagrant/git  
<br>
      
* cd
  - 디렉토리로 이동할 때 사용하는 명령어  
    [vagrant@host1 ~]$ cd git  
    [vagrant@host1 git]$
<br>
      
* ls
  - 디렉토리 내용을 나열하는 명령어  
    [vagrant@host1 git]$ ls  
    bitcamp-ncp  bitcamp-ncp2  bitcamp-study  
    [vagrant@host1 git]$  
<br>
      
* file
  - 파일 타입을 확인하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ file b.txt  
    b.txt: ASCII text  
<br>

* less
  - 파일 내용을 표시하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ less b.txt  
    1111  
    2222  
    3333  
    4444  
    5555  
    6666  
    b.txt (END)  
<br>
