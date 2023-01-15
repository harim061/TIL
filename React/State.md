# State

> 리액트는 필요한 것만 리렌더링 해줌

## React.useState()
```
const data= React.useState()
console.log(data)
```

![image](https://user-images.githubusercontent.com/90364684/212547248-189d8ac1-efa9-4056-81ea-602444633b5a.png)
- undefined : 초기값
- f() : data 값을 바꾸는 함수

❓ 연결 가능하지만 배열 형태는 불편

![image](https://user-images.githubusercontent.com/90364684/212547495-c0c53bfe-9906-4d88-be01-f0647d02066f.png)
![image](https://user-images.githubusercontent.com/90364684/212547502-76c08a34-088f-4c8e-8028-27fec22b6cc8.png)

💡 JS 이용하여 쉽게 배열에서 꺼내는 법
```
const food =["tomato","potato"]
const [myFavFood, mySecondFavFood] = food;
```
![image](https://user-images.githubusercontent.com/90364684/212548112-7762f79b-ec55-45d6-b46c-907f6f21ed6d.png)
