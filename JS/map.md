# map

> array에 있는 item을 내가 원하는 무엇이든지로 바꿔주고 새로운 array로 return

```
array.map()
```
![image](https://user-images.githubusercontent.com/90364684/213646045-0b465af5-c752-4c32-a37b-9e4b583bb923.png)

- 배열의 모든 item에 대해 실행됨
- 5개의 아이템 5번 실행
- ❌기존 배열 접근 불가능

```
array.map((item) => {item})
```
- 첫 번째 argument로 현재의 item을 가져올 수 있음

```
{toDos.map((item,index)=><li key={index}>{item}</li>)}

// {{item},{item},...}
```
- 리액트는 기본적으로 list에 있는 모든 item을 인식하므로 고유 키를 넣어줘야함
