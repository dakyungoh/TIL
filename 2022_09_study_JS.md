# 9월 13일
HTML과 Java Script의 만남

## script 태그
```
<h1>Java Script</h1>
<script>
 document.write('hello world');
</script>
```
HTML이 정적이라면 Java Script는 동적이다. (계산기처럼 작동할 수 있음)
'hello world' 자리에 수식을 넣으면 계산된 식이 나온다. 
```
<h1>Java Script</h1>
<script>
 document.write(1+1);
</script>
```
결과 : 

<img width="200" alt="스크린샷 2022-09-13 오후 10 16 45" src="https://user-images.githubusercontent.com/108469115/189911084-11dfe06f-7e5b-49e9-ab1b-6d5c7e31ca31.png">

## event 태그 : 사용자와 상호작용하는데 핵심적인 역할을 한다.(event=사건) 
```
</head>
    <body>
     <input type="button" value="hi" onclick="alert('hi')">
     <input type="text" onchange="alert('changed')">
     <input type="text" onkeydown="alert('key down!')">
    </body>
```
- input type="button" : 버튼을 만드는 태그
- value="hi" : 글자를 넣는 태그
- onclick="alert('hi')" : 클릭을 했을 때 'hi'라는 경고창을 넣는 태그(onclick의 속성값은 JS가 들어와야 한다)
- input type="text" : 글씨를 입력할 수 있는 태그
- onchange="alert('changed')" : 요소값을 변경하는 태그로서 클릭을 했을 때 'changed'라는 경고창으로 변경된다. 
- onkeydown="alert('key down!')" : 키를 누르면 'key down!'라는 경고창이 뜬다.

ex) onkeydown event의 결과 :

<img width="1009" alt="스크린샷 2022-09-13 오후 10 37 59" src="https://user-images.githubusercontent.com/108469115/189916011-7feb3165-21c8-4b21-a309-3a98618e41f1.png">

## Console (콘솔) 

