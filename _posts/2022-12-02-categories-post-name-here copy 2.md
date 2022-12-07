---
title: "[20일차] 프로그램 실행과 프로그래밍 - 2"
excerpt: " "

categories:
  - Categories2
tags:
  - [ ]

permalink: /categories2/post-name-here-12/

toc: true
toc_sticky: true

date: 2022-12-02
last_modified_at: 2022-12-02
---

## 🦥 수업 내용

**L1, L2 및 L3 캐시의 차이점: CPU 캐시는 어떻게 작동합니까?**

[https://quasarzone.com/bbs/qn_hardware/views/818208](https://quasarzone.com/bbs/qn_hardware/views/818208)

[https://woozzang.tistory.com/155](https://woozzang.tistory.com/155)

[https://sonb3579.tistory.com/15](https://sonb3579.tistory.com/15)

****캐시가 동작하는 아주 구체적인 원리****

[https://parksb.github.io/article/29.html](https://parksb.github.io/article/29.html)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cd5d06af-6400-41a6-a500-be41fc21aef9/Untitled.png)

- Web Browser와 JavaScript
    
    console=object 객체 .log=function ("출력1");=argument인자,parameter파라미터
    
    → web browser의 개발자 보드 콘솔창에 값을 출력하는 역할을 함
    
    ```
    <script>
      console.log("출력1");
      </script>
    ```
    
- 변수와 제어문
    - javascript 예제 1, 2
- Function (함수)
    - 특정 기능을 수행하도록 짜놓은 명령순을 묶어서 이름을 붙인것
        - 필요할때 언제든 재실행 가능!
        - 코드 재사용성을 높이는 문법
        
    - ****Popular Coding Convention on Github****
        
        [http://sideeffect.kr/popularconvention/#javascript](http://sideeffect.kr/popularconvention/#javascript)
        
- 함수 정의와 호출
    - 중첩 함수 호출
    - 함수 레퍼런스
- 객체와 프로퍼티
    - object 객체 : 덩어리
    - obj1 :  노트
        - var name = “홍길동”,
        - var age = “20”,
        - var warking = “false”,
        
        ```
        var obj2 = {
            name:"임꺽정",
            age:30,
            working:true,
            hello:function() {
              console.log("안녕하세요, " + this.name + "님!")
            },
        ```
        

- DOM API - getElementById()
    - DOM - Document / Object / Model
    - API - Application / Programming / Interface (App을 프로그래밍 할때 사용하는 도구)
    
    ⇒ 태그를 다루는 프로그램을 짤 때 사용하는 도구
    

- 객체와 함수=메써드=operator , 파라비터의 관계
    - 71page
- JavaScript와 ECMAScript 관계
- 요점 정리 - 5.HTML 태그와 DOM 트리 객체 응용
- 웹페이지 조립