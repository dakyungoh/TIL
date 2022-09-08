# 9월 7일

html을 사용하여 폰트 색상을 변경할 때는 변경할 모든 문구에 ```<font color="red">```를 입력해야 한다. 
```html
Hypertext Markup Language (HTML) is the standard markup language for <font color="red">creating</font> web pages.
CSS is a cornerstone technology of the World Wide Web, alongside HTML and <font color="red">JavaScript</font>.
```
<img width="1243" alt="스크린샷 2022-09-07 오후 2 36 33" src="https://user-images.githubusercontent.com/108469115/188796939-7b976b04-7ae9-41e8-ab49-aa46c5cb4acb.png">

## css의 style태그를 사용하면 모든 문구를 한번에 변경할 수 있다. 

색상은 빨강, 밑줄은 없이
```css
<style>
 a {
 color:red;
 text-decoration: none;
  }
 ```
 이 때 한 단어 및 문장만 변경하고 싶을 때에는 html 안에 style 속성을 사용하여 변경할 수 있다. 
 단, 새미클론(;)을 사용하여 구분을 지어주어야 한다. 
 ```
 <li><a href="2.html"style="color:orange;text-decoration:underline">CSS</a></li>
 ```
<img width="373" alt="스크린샷 2022-09-07 오후 3 03 34" src="https://user-images.githubusercontent.com/108469115/188800570-36cc2109-2088-44cf-8004-7b52ac717dfa.png">

```css
<h1> 위치의 속성을 변경할 때 : 글씨 크기는 45px, 가운데 정렬
 <style>
  h1 {
    font-size: 45px;
    text-align: center;
  }
  ```
  
 ## css에서 html의 속성을 주는 방법을 알아보자.
 용어 : 
 class : 어떤 의도에 의해 그룹으로 묶을 때 사용한다.  
  - ex) class값이 saw일 때는 .saw를 사용한다.
  
 id 선택자 : 우선 순위가 높은 것을 지정할 때 사용한다.
  - ex) id값이 active일 때는 #active를 사용한다. 
 
 이 때 값을 작성하는 순서가 중요하다. 
 태그 선택자 < class 선택자 (가장 마지막에 등장하는 선택자가 우선순위가 높다) < id선택자(단 한번만 등장해야 한다)
  1. id 선택자
  2. class 선택자
  3. 태그 선택자 
 <img width="530" alt="스크린샷 2022-09-07 오후 4 01 17" src="https://user-images.githubusercontent.com/108469115/188810938-dbe42146-b883-4277-a878-304d90dc0027.png">
  <img width="497" alt="스크린샷 2022-09-07 오후 4 00 17" src="https://user-images.githubusercontent.com/108469115/188810606-5ef9faeb-6b7b-4d5d-ba85-b9c7f3690052.png">
  
  실행결과 : 머물었던 HTML페이지 class에는 색깔 그레이를 지정하고, 머물고 있는 현재 페이지 CSS에는 레드라고 지정하였다. 
 
 <img width="140" alt="스크린샷 2022-09-07 오후 4 30 31" src="https://user-images.githubusercontent.com/108469115/188816589-87a281e0-e719-490e-87f2-1e1b724e5e4b.png">

# 9월 8일

박스 모델은 블록 레벨 요소(혼자 한 줄을 차지하는 것)와 인라인 레벨 요소(한 줄에 여러 개를 표시 가능)에 따라 나열 방법이 달라진다.  
```css
/*
block level element
*/
<h1>, <div>, <p> 등
```
```css
/*
inline level element
*/
<span>, <img>, <strong> 등
```
박스 모델은 콘텐츠 영역, 박스와 콘텐츠 영역 사시의 여백인 패딩(padding), 박스의 테두리(border), 여러 박스 모델 사이의 여백인 마진(margin)등의 요소로 구성된다.
박스를 만드는 법 : {border : 숫자px solid 색깔;}
콘텐츠 영역의 크기를 지정하는 속성
 - width : 너비
 - height : 높이
 
<img width="350" alt="스크린샷 2022-09-08 오후 2 42 01" src="https://user-images.githubusercontent.com/108469115/189043409-904d21ca-c8fc-4c09-9424-4d8f4171d361.png">
<img width="357" alt="스크린샷 2022-09-08 오후 2 42 51" src="https://user-images.githubusercontent.com/108469115/189043472-bc72519e-33d4-43c3-a1b7-9df25e62cd3e.png">

## 그리드를 사용하여 레이아웃을 설정해보자. 
1. div를 활용하여 그리드를 설정할 id를 정한다
 ```css
 ex)<div id="grid">
 ```
2. id 값을 활용하여 설정값을 지정해본다. 이 때 colums는 열을 의미한다. 1fr은 열의 크기를 지정할 수 있다. 
```css
 #grid{
    border : 5px solid gray;
    display: grid;
    grid-template-columns: 150px 1fr;
      }
 ```
 <img width="576" alt="스크린샷 2022-09-08 오후 3 59 30" src="https://user-images.githubusercontent.com/108469115/189055976-f20d2fcc-4b4b-427c-899d-0e7c158d25f1.png">
 <img width="623" alt="스크린샷 2022-09-08 오후 3 59 49" src="https://user-images.githubusercontent.com/108469115/189056025-df5672e8-5552-4fc5-bf7c-e0bf564f7904.png">

