# console.log로 계산기 만들기 
```
const calculater = {
    add: function (a, b) {
        console.log("a + b = ", a + b, "입니다");
    },
    minus: function (a, b) {
        console.log("a + b = ", a - b, "입니다");
    },
    multiple: function (a, b) {
        console.log("a + b = ", a * b, "입니다");
    },
    divide: function (a, b) {
        console.log("a + b = ", a / b, "입니다");
    }
}

calculater.add(32, 2);
calculater.minus(22, 1);
calculater.multiple(3, 2);
calculater.divide(10, 2);
```
![스크린샷 2022-10-14 오후 7 58 02](https://user-images.githubusercontent.com/108469115/195831187-89d8bfd9-0e6d-4f74-9840-990ad37e16bd.png)
