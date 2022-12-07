---
title: "[18일차] CSS 사용법"
excerpt: "CSS 사용법"

categories:
  - Categories2
tags:
  - [CSS]

permalink: /categories2/post-name-here-9/

toc: true
toc_sticky: true

date: 2022-11-230
last_modified_at: 2022-11-30
---

## 🦥 수업 내용
- CSS (이어서)
    - 예제 8-1 부터 ~ 테두리(
    
    ```html
    /* 테두리 다루기(border)
        => border-style : 테두리 모양
           예) solid, dashed, dotted 등
        => border-width : 테두리 두께
           예)thin, thick, 5px 등
        => border-color : 테두리 색상
           예) gray, rgb(100%, 0%, 0%), rgb(255, 0, 0), #ff0000
      */
    ```
    
    ```html
    /* 테두리와 여백 III
        => padding: 테두리 안쪽 여백
        => margin: 테두리 바깥쪽 여백
      */
    ```
    
    ```html
    /* display 속성 : block, inline, inline-block
        => block
           => 한 줄을 모두 점유한다.
           => 자신의 너비와 높이를 가질 수 있다.
           => 예) h1 ~ h6, div, p, address, ul, ol 등
        => inline
           => 한 줄 속에 포함되어 다른 태그와 그 줄을 함께 공유한다.
           => 자신의 너비와 높이를 가질 수 없다.
              콘텐츠의 크기에 따라 너비와 높이가 결정된다.
           => a, i, b, strong, span 등
        => inline-block
           => inline 처럼 한 줄을 다른 태그와 공유한다.
           => block 처럼 자신의 너비와 높이를 가질 수 있다.
      */
    ```
    
    ```html
    /*
        display: none
        => 출력 대상에서 제외시킨다.
        => 태그가 차지했던 영역은 사라진다.
    
        visibility: hidden
        => 출력 대상이 존재하지만, 화면에만 보이지 않게 한다.
        => 따라서 태그가 차지했던 영역은 그대로 둔다.
      */
    ```
    
- CSS와 js 분리하는 법

## 🦥 과제

  * naver.com의 메인 페이지를 똑같이 복제하라.
  * 팀구성
