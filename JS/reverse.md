# reverse

> 문자열 반대로 뒤집기

## 내장 함수들을 사용해 문자열 반전하기

- split() : 문자열을 부분 문자열로 구분해 여러 개의 문자열 배열로 분할
- reverse() : 배열을 반전
- join() : 배열의 모든 요소를 문자열로 결합

 ```
 var str = "hello";
 var splitString = str.split(str)
 // ["h","e","l","l","o"]
 
 var reverse = splitString.reverse()
 // ["o","l","l","e","h"]
 
 var join = reverse.join("")
 // "olleh"
 
 ```
