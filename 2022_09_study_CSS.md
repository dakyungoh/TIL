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
a {
 color:red;
 text-decoration: none;
}
``` 

---
이 때 한 단어 및 문장만 변경하고 싶을 때에는 html 안에 style 속성을 사용하여 변경할 수 있다. 
단, 새미클론(;)을 사용하여 구분을 지어주어야 한다. 

```
<li>
  <a href="2.html"style="color:orange;text-decoration:underline">CSS</a>
</li>
```

<img width="373" alt="스크린샷 2022-09-07 오후 3 03 34" src="https://user-images.githubusercontent.com/108469115/188800570-36cc2109-2088-44cf-8004-7b52ac717dfa.png">

---
`<h1>` 위치의 속성을 변경할 때 : 글씨 크기는 45px, 가운데 정렬
```css
h1 {
  font size: 45px;
  text-aline: center;
}
```
