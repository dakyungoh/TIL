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

# 9월 19일
Java Script 기초
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title></title>
    </head>
    <body>
      <h1>chaka babo</h1>
      <script>
        // --- 변수와 자료형
        var age = 1
        var name = 'chanhee'
        var isCute = true

        // --- 배열
        var names = ['egoing', 'chanhee', 'dakyung', 'kongdol']
        var ages = [40, 28, 27, 3]
        var cutenesses = [false, true, true, true]
        console.log(names[2])

        // --- 조건문
        console.log('-- 조건문 테스트 ---')
        // if (조건문) { 조건문이 참일 때 실행할 내용 } 
        // else { 위에 나온 조건문이 거짓일 때 실행할 내용} 
        if (isCute) {
          console.log('귀여워')
        } else {
          console.log('그닥')
        }

        // if (조건문1) { 조건문이 참일 때 실행할 내용 }
        // else if (조건문2) { 위에까지 나온 조건문들이 거짓이고, 방금 나온 조건문이 참일 때 실행할 내용} 
        // else { 위에 나온 조건문이 거짓일 때 실행할 내용} 
        var date = '7/3'
        if (date === '12/25') {
          console.log('야호 크리스마스다.')
        } else if (date === '5/5') {
          console.log('야호 어린이 날이다.')
        } else if(date === '1/1') {
          console.log('새해복 많이 받으세요.')
        }
        else {
          console.log('주륵 아무날도 아니다.')
        }

        // -- 함수 
        function getDiceValue() {
          // 주사위를 굴려서 1 ~ 6 사이 중 하나를 랜덤하게 받는 함수
          return Math.floor(Math.random() * 6 + 1)
        }

        // --- 반복문 (for & while loop)
        console.log('--- 반복문 테스트 1 - 이름 찍기 ---')
        // while과 for로 순회 반복해보기
        // 이 경우에는 for가 더 깔끔해 보인다.

        // while(조건문) { 조건문이 참일 때 실행할 내용 }
        var index = 0; 
        while(index < names.length) {
          console.log(names[index])
          index = index + 1;
        }

        // for(초기화 문장; 조건문; 조건에 변경을 가하는 문장) { 반복할 내용 }
        for (var i = 0; i < names.length; i = i + 1) {
          console.log(names[i])
        }

        // while과 for로 비순회 반복해보기
        console.log('--- 반복문 테스트 2 - 주사위 찍기 ---')
        // 이 경우에는 while이 더 깔끔해 보인다.
        var diceValue = 0
        
        while(diceValue !== 5) {
          diceValue = getDiceValue()
          console.log(diceValue)
        }

        for(var i = 0; i < Infinity; i = i + 1) {
          diceValue = getDiceValue()
          console.log(diceValue)
          if(diceValue === 5) {
            break;
          }
        }

        // 반복문은 중첩될 수 있다.
        console.log('-- 중첩 조건문 테스트: 환승연애 ---')
        var females = ['줄리엣', '춘향이', '공주님']
        var males = ['로미오', '몽룡이', '왕자님']
        for (var f = 0; f < females.length; f = f + 1) {
          for (var m = 0; m < males.length; m = m + 1) {
            console.log(females[f], males[m])
          }
        }

        console.log('-- 중첩 조건문 테스트: 구구단 ---')
        var numbers = [2, 3, 4, 5, 6, 7, 8, 9]
        for(var n = 0; n < numbers.length; n = n+1) {
          for(var m = 0; m < numbers.length; m = m+1) {
            console.log(`${numbers[n]} * ${numbers[m]} = ${numbers[n]*numbers[m]}`)
          }
        }

      </script>
    </body>
</html>
```
