---
title: "[15일차] HTTP 프로토콜"
excerpt: "HTTP, 네트워킹, Proxy 서버"

categories:
  - Categories2
tags:
  - [HTTP]

permalink: /categories2/post-name-here-7/

toc: true
toc_sticky: true

date: 2022-11-25
last_modified_at: 2022-11-25
---

## 🦥 수업 내용

* HTTP
  - 웹브라우저가 웹서버에게 연결 요청을함  
    
* 네트워킹
 1. Connection Oriented (연결지향)  
    1. 연결 후 통신  
       ex) 전화  
    2. 대표적 TCP  
       -데이터 전송 신뢰성 확보  
    3. statcful / stateless  
       -statcful ; 한번 연결한 후 연결을 끊을 때까지 여러번 통신  
         ex) ssh, FTP, 채팅, googlemeet  
       -단점 ; 많은 클라이언트에게 응답을 못함, 보완) 멀티쓰레딩 기술  
       -stateless ; 한번 연결에 한번 통신, 매번 연결  
        
2. Connectionless (비연결)
    1. 연결없이 데이터 전송  
        ex) 편지, 방송  
    2. 대표적 UDP  
        -데이터 전송 신뢰성 x → 별도의 처리 필요  
    
- HTTP
    - request line
        - **Method**
        
        ```
        | "GET"
        | "HEAD"                   
        | "POST"                   
        | "PUT"                     
        | "DELETE"
        ```
        
        - Status-Line
            - [https://www.w3.org/Protocols/rfc2616/rfc2616-sec6.html#sec6.1](https://www.w3.org/Protocols/rfc2616/rfc2616-sec6.html#sec6.1)
    - header
  
    - message-body
    
- Proxy 서버
    1. clinet와 sever 중간에서 통신을 중재
    2. 응답데이터를 보관 ⇒ 같은 자원을 요청할때 보관된 데이터를 즉시 전달 ⇒ 네트워크 오버헤드를 줄인다 ⇒ 응답속도 개선
    3. 모니터링 ⇒ 요청/응답 내용 감시 ⇒ 보안 강화
    4. URI
        1. URL (-locator)
        2. URN (-name)
    5. Get 요청
    6. text vs binary 파일
        1. text - 일반 텍스트 편집기로 편집 가능한 포맷
            1. 예) txt, rtf, html, css, js 등등
        2. binary - byte 단위로 포맷 / 일반 텍스트로 편집 불가 / 전용 app.사용
            1. 예) jpg, mp3
            2. 텍스트로 인코딩해서 보내면 가능함 base64로 변경해서 보여주기
                1. 
                
                [URL length: how long can a URL be? - SISTRIX](https://www.sistrix.com/ask-sistrix/technical-seo/site-structure/url-length-how-long-can-a-url-be)
                
    7. POST 요청
        1. POST /html/form/exam02
        2. 특징) binary 데이터 전송 가능 / url에 노출 안됨
