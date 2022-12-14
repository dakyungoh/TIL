# 9월 1일

코드 설명: 텍스트를 꾸미고 싶으면 HTML Tags 를 아래처럼 이용하면 된다. 
```html
Hypertext Markup Language (HTML) is the standard markup language for <strong>creating <u>web</u> pages</strong>.
```

방법: 
```html
<strong>글자 진하게</strong>
<u>아래 밑줄 긋기</u> 
```

실행 결과: 

<img width="1019" alt="스크린샷 2022-09-02 오후 5 38 47" src="https://user-images.githubusercontent.com/108469115/188099960-b72874db-a27d-4bb9-989c-942f99379d75.png">

# 9월 2일

코드 설명 : 텍스트에 색칠을 하고 싶으면 style 속성을 사용한다. 값으로는 css를 받는다. 나중에 공부하자.
```html
Hypertext Markup Language (HTML) is the standard markup <span style="color:Green">language</span>
```
  
방법: 
```html
<span style="color:green">색칠된 글자</span>
```
  
실행 결과:
  
<img width="607" alt="스크린샷 2022-09-02 오후 6 06 05" src="https://user-images.githubusercontent.com/108469115/188105428-a29fea20-3a78-45bb-a8ca-e607202ddca2.png">

  
# 9월 4일

## 맥에서 터미널 사용법
command 익히기 : 
- ls : 현재 디렉토리에 있는 파일과 디렉토리를 본다.
- cd ${dir}: 다른 디렉토리로 이동한다. 
- cd .. : 부모 디렉토리로 이동한다. 
- mkdir : 새로운 디렉토리를 만든다.
- echo > ${filename}: filename이라는 파일을 만든다. 
- open . : 현재 디렉토리를 파인더에서 연다. 
- code . : 현재 디렉토리를 vs코드에서 연다. (설치필요: command + shift + p)

## git command 기초

![128hsgntnsu9bww0y8sz](https://user-images.githubusercontent.com/108469115/188307706-b3b23cd7-1760-43fa-afef-c4d57a320861.jpeg)

- git status : working directory와 staging area의 차이를 확인한다. 
- git add ${add할 파일 이름}: working directory의 수정사항을 staging area에 올린다. 
  - git add . : 모든 수정사항을 올릴 때 사용!
- git commit -m "커밋 메시지" : staging area의 현재버전을 내 컴퓨터 상의 레포지토리(local repo)에 올린다.
- git push : local repogitory의 현재버전을 remote repo(깃허브의 레포지토리)에 올린다. 
- git clone ${clone할 레포 주소} : 특정 레포지토리를 복제해온다. 
- git pull : remote repo에서 현재버전을 당겨온다. 

# 9월 5일
코드 설명 : 텍스트를 heading(큰 제목) 하려면 HTML Tags 를 아래처럼 이용하면 된다.
          문장과 문장을 나누는 단락/줄바꿈을 사용하는 HTML Tags를 사용할 수 있다.

```html
<h1>HTML</h1>
Hypertext Markup Language (HTML) is the standard markup language for <strong>creating <u>web</u> pages</strong> and web applications.
<img src="./images/coding.jpg" width="50%">
<p>
  HTML elements are the building blocks of HTML pages. With HTML constructs, images and other objects, such as interactive forms, may be embedded into the rendered page.
</p>
It provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other items. 
<br>
HTML elements are delineated by tags, written using angle brackets.
<br>
```

방법: 
```html
<h1>큰 제목</h1>
<P>단락</P> 
혹은 
<br>단락
<img src="./images/coding.jpg" width="50%">
```

실행 결과:

<img width="852" alt="스크린샷 2022-09-05 오후 9 13 29" src="https://user-images.githubusercontent.com/108469115/188446739-06ad4cba-8fe4-43a1-95e1-2548a2c9417c.png">

# 9월 6일

``` 
list item의 줄임말 : <li></li>
순서 없는 목록을 사용할 때 만든다(unordered list의 줄임말) : <ul></ul>
```
<img width="583" alt="스크린샷 2022-09-06 오후 4 36 05" src="https://user-images.githubusercontent.com/108469115/188574800-9b297e4a-ed4b-4096-a6df-52d3b44a69aa.png">

```
순서있는 목록을 사용할 때 만든다(ordered list의 줄임말) : <ol></ol>
```
<img width="568" alt="스크린샷 2022-09-06 오후 4 36 46" src="https://user-images.githubusercontent.com/108469115/188574940-e0978be2-9ddf-4fdc-8088-7fee6a4dfdd5.png">
```

## 1. 문서 유형 지정하기
```
첫번째 줄에 <!DOCTTPE html>소스 입력하기 
```
입력해야 하는 이유 : 브라우저가 해당 파일이 html로 이루어져 있다는 것을 알 수 있게 하기 위해서 

## 2. <html>태그 입력하기 
```
웹 문서 시작과 끝은 각각 <html>과 </html>로 표시해야한다.
```

## 3. <head>,<meta>,<title>,<body>태그 입력하기
```
<head> : <head>와 </head> 태그 사이에는 문자 세트와 문서 제목을 입력할 수 있다. / 웹 문서의 정보를 저장
<meta> : 문자 세트를 지정한다. ex)<meta charset="utf-8">
<title> : 웹 문서의 제목을 입력한다. 
<body> : <body>태그는 </head>태그 다음 줄에 입력한다. <body>와 </body> 사이에 <h1>등 다양한 태그를 추가할 수 있다. / 웹 브라우저에 보여 줄 내용을 저장
```
  
## 4. 링크
```
<태그이름 속성명1=“속성값1” 속성명2=“속성값2”>화면에 표시할 값</태그이름>
<a href="https://www.naver.com" target="_blank">링크로 연결될 문장</a> 
```
## 5. 내가 만든 웹 사이트 
https://dakyungoh.github.io/my-first-web-site/
  
