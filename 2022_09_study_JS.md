# 9월 13일
HTML과 Java Script의 만남

## script 태그
```html
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

# 9월 14일

## 데이터 타입 - 문자열(string)과 숫자(number)
- 산술 연산자 : 수식에서 사용되는 사칙연산 '+,-,*,/'을 의미한다. 
- 문자열(string) : "글자" , '글자' 
- 숫자 1+1 =2 / 문자열 "1"+"1"= "11"   
- 문자열(string) : "글자" , '글자' 
ex) 'Hello World' . length : ''Hello World'의 글자수를 알 수 있다. 
ex) 'Hello World' . toUpperCase() : ''Hello World'를 'HELLO WORLD' 라고 대문자로 바꿔준다. 
ex) 'Hello World' . indexOF('world') = 6 : ''Hello World'에서 'world'는 6번째에 있다. 
ex) '       Hello World      ' . trim() = 'Hello World" : 공백을 없애준다. 

## 변수와 대입 연산자 
```
x = 1;
x : 변수(variable) 
= : 대입연산자 
변수의 반대말은 상수(constant)
```
ex) var name = 'kongdol'; 
-> 이름을 'kongdol'로 바꾸어 달라! 
수정할 이름에 +name+ 이라고 작성하면 된다. 

# 9월 16일

## 제어할 태그 선택하기
'night' 버튼을 눌렀을 때 배경색깔은 검정, 글자색깔은 하얀색으로 만든다. 
```javascript
<input type="button" value="night" onclick="
  document.querySelector('body').style.backgroundColor = 'black';
  document.querySelector('body').style.color = 'white';
 ">
```
결과 : 

<img width="739" alt="스크린샷 2022-09-16 오후 9 28 59" src="https://user-images.githubusercontent.com/108469115/190638864-825f4ffc-aaf6-4cd5-9f19-f2de3b8b8706.png">

## 데이터 타입 - boolean(논리학에서 참과 거짓을 다루는 용어)과 비교 연산자
boolean : true & false를 구분할 수 있는 데이터 타입

<img width="342" alt="스크린샷 2022-09-16 오후 10 00 07" src="https://user-images.githubusercontent.com/108469115/190644635-40e2a654-b2c9-446a-93ac-1fbe4341fa5c.png">
여기서 1&lt2는 1<2와 같은 뜻이다. 
