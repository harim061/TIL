> https://react-tutorial.app/app.html

# 1. intro

## 1-1. Uppercase a string
>  문자열을 대문자로 변환해서 반환

```
string.toUpperCase()
```
- 인자 ( Parameters )  -> 없음
- 반환값 ( Return) -> 대문자로 반환된 문자열


## 1-2. Array.filter recap
 > 주어진 함수의 테스트를 통과하는 모든 요소를 모아 새로운 배열을 반환

```
const grades = [10,2,21,-10];
const result = grades.filter(grade => grade > 20);
// [21]
```
### JSON ( JavaScript Object Notation )
> JS 객체 문법을 따르는 문자 기반의 데이터 형식

```
{
    “name” : “kim”,
    “num“ : 1
}
``` 
위의 객체는 사람을 나타냄
여러 사람이 존재하는 경우?
### 객체가 존재하는 배열 생성하기

```
let people = [
{ 
    “name” : “kim”,
     “num” : 1
},
{
    “name” : “lee”,
    “num” : 2
}
]
```
여러 사람을 다음처럼 같은 배열로 표현 가능

### 배열 내 특정 값을 만족하는 객체 찾기
#### Array.find 메서드 사용하기
~~~
let person = people.find(person->person.name ===“kim)
// {name:kim, num : 1}
~~~



