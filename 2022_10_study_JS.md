# console.log로 계산기 만들기 
```
const calculater = {
    add: function (a, b) {
        console.log("a + b = ", a + b, "입니다");
    },
    minus: function (a, b) {
        console.log("a - b = ", a - b, "입니다");
    },
    multiple: function (a, b) {
        console.log("a * b = ", a * b, "입니다");
    },
    divide: function (a, b) {
        console.log("a / b = ", a / b, "입니다");
    }
}

calculater.add(32, 2);
calculater.minus(22, 1);
calculater.multiple(3, 2);
calculater.divide(10, 2);
```
![스크린샷 2022-10-14 오후 8 42 50](https://user-images.githubusercontent.com/108469115/195838843-81213581-69b5-49e2-b61b-9156f7a5bbdd.png)
