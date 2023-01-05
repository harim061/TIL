# user-defined name

1. 객체의 도움을 받아 만들기
```
let my_var = "userVariable":
let my_value = "userValue";

let x ={
  [my_var] : my_value,
  };
console.log(x);
console.log(x[my_var]);
```
userVariable : userVaule

userValue

2. this 키워드 사용
```
let my_var = "userVariable":
let my_value = "userValue";

this[my_var] = my_value;

console.log(my_var);
console.log(this.[my_var]);
```
userVariable

userValue
