# JSON
> JSON은 JavaScript Object Notation의 약자로, 브라우저와 서버사이에서 오고가는 데이터의 형식


## JSON.stringify
> JSON 문자열로 반환

```
JSON.stringify(value, replacer)
```
- value : JSON 문자열로 변환할 값. 배열, 객체, 등

- replacer: 함수 또는 배열 (기본 값 = 문자열)

![image](https://user-images.githubusercontent.com/90364684/211164610-8594242b-a0bf-48e6-867d-0217f357baaa.png)

![image](https://user-images.githubusercontent.com/90364684/211164597-7b4614e5-b939-4f1f-a42e-a457d9ff8041.png)

문자열로 변환 


❓ JSON은 string format만 지원 stringify도 string만 지원 둘의 차이는?

```
const todo = ["hi","hello"];
localStorage.setItem('todo',todo)
localStorage.getItem('todo')
```
"hi,hello" 

✅ 리스트 형식 없애고 내용물만 string화

```
localStorage.setItem('todo',JSON.stringify(todo))
localStorage.getItem('todo')
```
'["hi","hello"]'

✅ 리스트 형식 그래도 string화

## JSON.parse("[1,2,3,4]")
> JSON 문자열을 JSON 객체로 변환 

![image](https://user-images.githubusercontent.com/90364684/211207600-1eed15e7-fbe3-4e4d-b7db-47adb39291de.png)

![image](https://user-images.githubusercontent.com/90364684/211207697-2189a4c5-bfe5-48fe-8ee0-0aaf666ba868.png)
