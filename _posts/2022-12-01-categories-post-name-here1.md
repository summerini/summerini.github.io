---
title: "[19일차] 자바스크립트?"
excerpt: "JavaScript에 대해 알아보자"

categories:
  - Categories2
tags:
  - [JavaScript]

permalink: /categories2/post-name-here-10/

toc: true
toc_sticky: true

date: 2022-12-01
last_modified_at: 2022-12-01
---

## 🦥 수업 내용

- 라이브러리 설명
- 프로그램 실행과 프로그래밍
    - 사용자 → app → OS → 컴퓨터 → 모니터

1) app→os 읽기

2) os→컴퓨터(ram) 저장

3) ram→컴퓨터(cpu) 전달

4) cpu 명령어 실행

5) cpu→ram 전달

6) ram→os 결과 꺼내기

7) os→모니터 화면출력

#app → compter 읽기~저장 (”loading”)

#개발자→app (”Programming”)

---

 * 포팅

○ 사전적 의미

1. 이식(移植) ((다른 기종의 컴퓨터로 소프트웨어를 옮기기))
2. [컴퓨터] 포팅(porting), 특정 운영 체제용 소프트웨어를 다른 운영 체제에서 작동시키기 위해 변경하는 것
3. 옮겨심기, 식물을 다른 장소로 옮겨 심는 것.

○ 업무에서 의미

1. 특정 운영체제용 소프트웨어를 다른 운영 체제에서 작동시키기 위해 변경하는 것

---

 * cpu / ram

- cpu ↔ ram
    - cpu→결과 데이터, ram→데이터, 명령
    - 선 갯수(bit) → 8,16,32,64 bit
- cpu 제조사는 cpu를 통해 명령을 실행시키는 방법을 명세서로 제공한다
    - 신호 보내는 비트 규칙 instruction set (데이터 셋)
    - cpu 버전이 업그레이드 되면 명령 규칙이 추가된다
    - cpu 마다 명령어 다름 : ex) intel i계열 제온계열
    - cpu 제조사 마다 명령어 다름 (전기 신호를 보내는 규칙

---

- 명령어 작성
    
    1. cpu instruction set 명세서를 보고 직접 명령어 작성
    - 특징
        - cpu bit가 작은 8bit 시절에는 개발자가 직접 작성하기도 했다
        - 보통 2진수를 짧게 표현한 16진수를 사용해서 작성한다
        - 인간의 문자와 거리가 멀기 때문에 작성하기 매우 불편하고 힘들다
        - cpu bit가 32bit, 64bit로 늘어나면서 더 어렵게 되었다
        - cpu 회사 명령어가 다르게 때문에 다양한 cpu에서 실행할 수 있는 명령어를 작성하기 매우 힘들다
    1. Assembly
        1. 직접 기계어로 작성하는 대신 간결한 영어 단어로 이루어진 명령어 사용하기
            1. 개발자→ (작성) → assembly → (변환)compile → 기계어 →(cpu instruction set) → (실행) → cpu
            *compile - assembly언어로 작성된 명령어를 cpu가 이해할 수 있는 기계어로 바꿔주는 프로그램
    - 특징
        - 명령어 영어 단어와 비슷해서 작성하기 편하다
        - cpu마다 다르게 작성할 필요가 없다 → why? 컴파일러가 cpu에 맞춰서 기계어로 번역해줌
    1. C언어
        1. 더 인간 친화적인 프로그래밍 언어로 명령어 작성하기
            1. 개발자→ (작성) → c → (변환)c compile → 기계어 →(cpu instruction set) → (실행) → cpu
- 기계어, OS, CPU
- C 컴파일
    - hello.c → gcc컴파일러 (gcc hello.c) → a.out
        - a.out - windows XX intel cpu 기계어로도 명령문의 배치 방법이 다르기 때문에 windows에서는 인식할 수 없다
        - .exe - wimdows 에서 사용이 가능한 c 컴파일러 생성
    - 예전의 프로그램 공유 문화
        - 소스코드를 그대로 공유 - cpu가 달랐다
        - 컴파일해서 프로그램을 사용하는것이 일방적이다
    - C컴파일 + OS 전용 명령 사용
- 프로그래밍 언어와 컴파일러
    - 개발자 언어 선택?
        - C언어
        - C++언어
        - Pascal언어
    - 프로그래밍 언어마다 특장점이 있다
        ⇒프로젝트 성격에 따라 언어를 선택해야한다
        
- 컴파일 방식과 인터프리트 방식
    - 컴파일 방식
        - 실행할때 기계어 파일만 있으면 된다
        - 소스파일 필요없음 → 소스파일을 보호할 수 있음(자산)
        ⇒ 기계어 바로 실행, 실행속도 빠름
        
    - 인터프리트 방식
        - nodejs 컴파일 하지 않는다
        - 실행할때마다 소스 파일 필요
        - 소스파일 공개 → 자산으로 보호하기 힘들다
        ⇒ 매번 명령어를 해석해서 실행, 실행속도 느림
        
- 인터프리터
    - 대표 ; viewer = player = engine =
    !이 파일을 열 때 사용할 앱을 선택하세요 = 읽어서 실행할 플레이어를 선택하라는 뜻
    
- javascript engine
    - 설치 :
- Webkit - html,css 렌더링 엔진
    - 구역 <html>…<script>…javascript 코드
- V8 - 오픈소스로 공개됨
    - V8 + @ = nodejs (standalone javascript engine)
        - 웹 브라우저 없이 단독으로 실행함
        - 구역 상관 없음
        - 데스크탑용 javascript player
        
        ***LTS 버전**
        - **C:\Users\bitcamp>echo %path%**
            **프로그램이 있는 경로 찾기**
        - **C:\Users\bitcamp>"c:\Program Files\nodejs\node" -v**
            **경로 프로그램 실행 하기**
            
        - 시스템 환경 변수 편집 → path 편집 → 새로만들기 → 경로 설정 **c:\Program Files\nodejs**
- JIT Compile과 AOT Compile
    - Plain 인터프리터 ⇒ JIT 컴파일
- Android와 App, AOT Compile
    - App을 설치할때 해당 Cpu에 맞춰서 컴파일 한다 “AOT”컴파일
    - bytecode:진짜 기계어가 아니라 기계어에 흡사한코드 ”중간코드”⇒P-code (초벌구이)
- Web Browser와 JavaScript
    - JavaScript 명령문이 아니라 코드


## 🦥 과제

  1. naver.com의 메인 페이지를 똑같이 복제하라. (완성까지)  
  
  
  
