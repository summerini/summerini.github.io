---
title: "[13일차] Web 기술 소개와 프로그래밍 기초"
excerpt: "두둥 HTML, HTTP의 등장"

categories:
  - Categories2
tags:
  - [Web]

permalink: /categories2/post-name-here-4/

toc: true
toc_sticky: true

date: 2022-11-23
last_modified_at: 2022-11-23
---

## 🦥 수업 내용

* Web 기술 소개 (HTML, HTTP 등장 배경)  
* FTP (File Transfer Protocol) - 논문 파일을 송수신하기 위해 사용했던 규칙  
  - Text 업로드 → FTP Sever → (통신) FTP client
  - 통신 규칙에 따라 data를 송수신 = 통신규칙 (protocol)
  - 단점  
    -논문이 참조하는 다른 논문을 다운로드 받기 번거롭다  
    -논문 안에 다른 논문이 업로드된 서버 주소가 없다  

* HTML (Hyper-Text Markup Language)  
  - Text에 별도의 표시를 함 / HTML 태그  
  - 다른 논문의 위치 정보 삽입 + 텍스트의 포맷을 지정 + 그림, 음성, 동영상 삽입  
예) <a href=”서버/a/t. html”> 제 1논문 </a>  
      <img src=”a. gif”>  
데이터를 설명하는 데이터 / 데이터를 제어하는 데이터 ⇒ 부가 데이터 ( metadata=markup  

* HTTP (Hyper-Text Transfer Protocol)  
  - HTTP 프로토콜을 통해 HTML 논문을 HTTP 클라이언트  
  - Hyper-Text / Transfer / Protocol  
  - HTML 문서를 원활하게 받고 다른 HTML 문서를 찾아가기 쉽도록 만든 통신 프로토콜  
  - HTTPS (Hyper-Text Transfer Protocol Security)

* 프로그래밍 기초
  * 데이터와 메모리 관계  
  * 10진수, 2진수, 16진수  
[![하버드 데이터 강의](https://img.youtube.com/vi/nvO1sq_b_zI/0.jpg)](https://youtu.be/nvO1sq_b_zI)

* 예제소스 다운로드  
  - [모던 웹을 위한 HTML5+CSS3 바이블(3판)]
  - https://www.hanbit.co.kr/support/supplement_list.html  
<br>
## 🦥 과제

* 웹 기술의 등장과정을 조사하여 설명하시오.  

* 웹기술의 등장 과정:

1. 어느 단체의 누가 어떤 목적으로 웹 기술을 만들었는지?  
    1. Timothy Berners Lee는 CERN(유럽 핵 연구소)에서 과학자들의 정보를 관리하고 연구성과를 쉽게 공유할 수 있도록 하기를 원했고 이를 통해 연구 생산성을 높일 수 있을 것이라고 생각했다.  
그래서 그는 HTTP, HTML, URL 등 현재의 인터넷 브라우저를 구성하는 기술들을 고안해내었다. 최초로 만들어진 웹 페이지는 1991년 8월에 만들어진 CERN의 홈페이지였고 기본적인 틀이 갖춰지게 된 이후 핵심적인 기술들이 발명되어 왔다.  

2. 웹 기술의 처음 목적과 지금 활용되는 상황이 어떻게 다른지?  
    1. WEB 1.0  
    -WWW라 불리는 그것  
    -단순한 문서의 구조를 표현하는 형태로 등장  
    -지금 사용하는 웹과는 차원이 다른, 문서의 구조를 표현하기만 하는 시대  
    -HTML을 통해 문서 구조를 표현  
    -주로 텍스트와 링크로 구성  
    -하이퍼링크 기능을 통해 전세계 페이지를 통합  
    -정적인 형태  
    2. WEB 2.0
    -웹사용자들이 웹 콘텐츠를 만들어나가는 적극적인 자세로 변화  
    -동적인 형태의 기술 등장  
    -기존 언어들의 단점을 보완해 다양한 기술을 제공해주는 언어들이 등장  
    -CGI (Common Gateway Interface)의 등장으로 입력이 함께 등장  
    -이러한 입력값 (ID, 패스워드)을 통해 전달되는 값을 변조할 수 있게 되어 취약점으로 이어짐  
    3. WEB 3.0
    -Semantic Web : 페이지를 태그를 통해서 각각의 의미를 부여할 수 있는 기능  
    -HTML5 + Javascript + CSS3만으로 프로그램 구현가능  
    -복잡한 구조의 웹이 등장하면서 성능뿐만 아니라 보안도 강화됨  
    -과거에는 서버 (back-end)가 필수였지만 지금은 웹만으로 프로그램 구현가능  
    ![www](https://user-images.githubusercontent.com/118426890/204127290-8b4d0387-7c6d-4633-8607-59b3a9ad5f98.png)
