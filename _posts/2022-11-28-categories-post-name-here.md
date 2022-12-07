---
<<<<<<< HEAD
title: "[16일차] Web 기술 - 1 "
excerpt: " "
=======
title: "[16일차] Web 기술 (HTML, CSS)"
excerpt: "HTML, CSS 사용법"
>>>>>>> cfcbdb6a37376ed5e54833396d835e7ddd2616cb

categories:
  - Categories2
tags:
<<<<<<< HEAD
  - [ ]
=======
  - [HTML], [CSS]
>>>>>>> cfcbdb6a37376ed5e54833396d835e7ddd2616cb

permalink: /categories2/post-name-here-8/

toc: true
toc_sticky: true

date: 2022-11-28
last_modified_at: 2022-11-28
---

## 🦥 수업 내용

<<<<<<< HEAD
* - CSS 사용법
    - CSS - Cascading Style Sheet : HTML element의 모양을 정의
    
    body ← style (size)
    
    h1 ← style (size, background)
    
    selector → 스타일을 적용할 대상을 가리킨다.
    
    Pseudo selector (대상의 상태)
    
    `.content header > span.title:hover {` 
    
    `background-color : red;`
    
    `color : white ;`
    
    `}`
    
    style name
    
    style value
    

**1) selector 사용법**

**2) specificity (스타일 적용 순서)**

3) box 다루는 방법 (테두리, 여백, 박스 계산법)

4) 폰트 다루는 방법

5) 색상 지정하는 방법

6) 배경 다루는 방법

7) block과 inlme 다루는 방법

8) 위치 조정하는 방법

- 셀렉터 { 스타일:값; 스타일:값; … } selector

{ ㅡ }

태그명 { ㅡ }

태그명, 태그명, 태그명 { ㅡ }

*그룹명 { ㅡ } class

#태그아이디 { ㅡ }

ㅡ[속성명=값] { ㅡ }

-:상태명 { ㅡ } pseudo selector

-body의 기본 margin이 있어서 margin을 없애려면 명확하게 0px로 설정해야함

-각 div의 위아래 margin은 겹쳐짐 (10+10 = 20이어야하는데? 10으로함)

- 부모 태그와 자식 태그의 계층 구조

html 

  body

    div

     h1

      p

TodoMVC

React Vue.js AngularJS

[stackoverflow.com](http://stackoverflow.com/) 

-display: none (content를 숨길때 사용함)

-“c1 c2” (그룹 class에 소속된 순서에 대해서는 영향을 끼치지 않음, 단 style에 대한 순서에 대해서는 순서대로 적용됨)

-대상자의 상태를 지정하기 : 의사 셀렉터(pseudo selector)

-:hover (맴돌다) li 태그 위에 마우스 커서가 대상자 위에 있는 상태

border

[https://www.w3.org/TR/CSS2/box.html#border-properties](https://www.w3.org/TR/CSS2/box.html#border-properties)

|| or 표시

Inherited. yes/no (상속되어있는지를 확인함)

테두리/색상/폰트

- 

```
/* 실렉터(selector) II
     자손태그 지정
     => 특정 대상자를 조상으로 갖는 태그를 지정하는 방법
     => 문법
        조상대상자 적용할자손대상자 {...}
```

```html
/* 실렉터(selector) II
     자식태그 지정
       => 특정 대상자를 부모로 갖는 태그를 지정하는 방법
       => 문법
          부모 > 적용대상자 {...}
   */
```

```html
/* 실렉터(selector) II
     특정 대상자 다음에 오는 태그를 지정하기
     => 특정 대상자를 바로 위의 형으로 갖는 경우.
     => 문법
        형 + 다음동생대상자 {...}
img + ul 
손주태그가 아니라 이미지 바로 다음 자식 태그에 한해서 해당함
```

```html
/* 실렉터(selector) III
     특정 조건을 갖는 대상자를 지정하기
     => 대상자를 지정할 때 조건을 나열할 수 있다.
     => 문법
        대상자#아이디 {...}
        대상자.분류명 {...}
        대상자:상태명 {...}
        대상자[속성명] {...}
더블 쿼테이션 적어주기 ""
input[type="text"] {
    background-color: yellow;
  }

/* selected 속성의 값에 상관없이 해당 속성이 있는 경우*/

  input[type="text"][value] {
    border: 3px solid red;
  }
```

```html
버튼 만들기
<input type="submit" value="전송버튼">
<input type="reset" value="초기화버튼">
<input type="button" value="일반버튼"><br>

요즘트렌드임 -> ->
<button type="submit">전송버튼</button>
<button type="submit">초기화버튼</button>
<button type="submit">일반버튼</button>
```

```html
input[name^="office"] { /* 속성의 값이 특정 문자열로 시작하는 경우*/
    background-color: yellow;
  }
```

```html
input[name$="fax"] { /* 속성의 값이 특정 문자열로 끝나는 경우*/
    color: red;
  }
```

```html
a:visited {
    color: gray;
  }

방문한적이 있는 사이트는 gray 지정
```

```html
a:active {
    background-color: yellow;
  }

링크를 클릭했을때 변경하고 싶을때 사용
```

```html
a:focus {
    border: 2px inset red;
    font-size: 150%;
  }

```

ctrl + / 주석 막기

```html
/* 스타일 적용 순서
    => specificity 값?
       => 실렉터의 우선 순위를 지정하기 위해 부여된 값
       => 한 태그에 같은 스타일이 중복 지정된 경우?
          specificity 값을 계산하여 값이 높은 스타일이 적용된다.
          스타일을 선언한 순서 보다 계산 값이 우선한다.
       => specificity 계산법
       *              : 0
       태그           : 1
       클래스, 조건   : 10
       아이디         : 100
       인라인스타일   : 1000
   */
```

- CSS specificity : 스타일 적용순서 낮→높
- html 백그라운드컬러는 되도록 지정하지 않는걸로함 / 와일드카드 사용은 가능한 하지 않도록함 * { } → 변수가 많음 ⇒ 되도록 body부터 사용함

- 태그의 너비, 높이
    - block 태그 = 너비, 높이 설정 가능
    - inline 태그 = 너비, 높이를 임의적으로 바꿀수없음
    
    ```html
    /* font-size 스타일은 자식태그에게 상속해 준다.
       자식 태그는 자체적으로 지정된 스타일이 없으면
       부모 태그로부터 상속 받은 스타일을 사용한다. */
    ```
    
    ```html
    /* = 1 */
    /* 같은 점수일 때 나중에 지정된 스타일이 기존 스타일을 덮어쓴다 */
    xdiv { 
      width: 200px; 
      background-color: green; 
    }
    
    /* = 1 */
    div { 
      background-color: navy;
    }
    
    /* = 10 */
    .c1 { 
      background-color: orange;
    }
    
    /* = 100 */
    #d2, #d3 { 
      background-color: red;
      color: blue;
    }
    
    /* = 1 + 100 = 101 */
    div#d3 {  
      background-color: skyblue;
    }
    
    #d3보다 div#d3가 우선순위가 더 높음
    ```
    
- get/post 요청
    - html ⇒ form - 3,4,5
    
    **<option value="a" selected>A형</option>**
    
    selected=”selected” 값은 브라우저에서 무시함
=======
* Web 기술
>>>>>>> cfcbdb6a37376ed5e54833396d835e7ddd2616cb
