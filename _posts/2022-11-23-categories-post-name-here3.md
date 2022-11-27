---
title: "[13일차] 명령어를 다루는 명령어"
excerpt: "type, which, man, apropos, info, whatis, alias"

categories:
  - Categories2
tags:
  - [Linux]

permalink: /categories2/post-name-here-3/

toc: true
toc_sticky: true

date: 2022-11-23
last_modified_at: 2022-11-23
---
## 🦥 과제
* type, which, man, apropos, info, whatis, alias
* 명령어를 다루는 명령어에 대한 설명과 사용 예시, 출력 결과 일부를 알아보자
<br><br><br>

## 🦥 명령어를 다루는 명령어
* type
  - 지정된 명령어가 쉘에 내장된 명령어인지 외부명령어인지 앨리어스 명령어인지 등을 확인하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ type d.txt  
    bash: type: d.txt: not found  
<br>

* which
  - 명령어의 경로를 확인하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ which ls  
    alias ls='ls --color=auto'  
        /usr/bin/ls  
<br>

* man
  - 각종 명령어, 프로그램의 매뉴얼을 확인하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ man ls  
    [vagrant@host1 bitcamp-ncp]$  
<br>

* apropos
  - 검색어와 관련이 있는 명령어를 설명과 함께 출력하는 명령어  
    [vagrant@host1 bitcamp-ncp]$ apropos rm  
    sysinfo (2)          - returns information on overall system statistics  
    Config (3pm)         - access Perl configuration information  
    Pod::Perldoc (3pm)   - Look up Perl documentation in Pod format.  
    Pod::perldoc (3pm)   - Look up Perl documentation in Pod format.  
    _Exit (2)            - terminate the calling process  
    _Exit (3p)           - terminate a process  
    _exit (2)            - terminate the calling process  
    _exit (3p)           - terminate a process  
    abort (3)            - cause abnormal process termination  
<br>

* info
  - 리눅스 명령어의 사용 방법 옵션등을 나타내는 명령어  
    [vagrant@host1 bitcamp-ncp]$ info pwd  
<br>

* whatis
  - 명령어에 대한 기능을 간략하게 나타내주는 명령어  
    [vagrant@host1 bitcamp-ncp]$ whatis pwd  
<br>

* alias
  - 별칭이란 뜻으로 사용자가 명령어를 다른 이름으로 바꿔서 사용할 수 있는 명령어  
    [vagrant@host1 bitcamp-ncp]$ alias  
    alias egrep='egrep --color=auto'  
    alias fgrep='fgrep --color=auto'  
    alias grep='grep --color=auto'  
    alias l.='ls -d .* --color=auto'  
    alias ll='ls -l --color=auto'  
    alias ls='ls --color=auto'  
    alias which='alias | /usr/bin/which --tty-only --read-alias --show-dot --show-tilde'  
<br>
