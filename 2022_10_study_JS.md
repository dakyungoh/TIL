- console.log로 계산기 만들기 
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
