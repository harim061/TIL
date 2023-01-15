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

### ❓리렌더링 해주기
> React.useState() 배열이용

> data는 원하는 이름, f는 set+데이터이름

![image](https://user-images.githubusercontent.com/90364684/212549171-da380f0d-1126-4d0e-848c-9402c0f72f55.png)

💡 값을 부여하면 setCounter 함수는 그 값으로 업데이트, 리렌더링 일으킴

#### state 값 할당하는 법
1. 직접 할당 : setCounter( counter +1 )

```
setCounter(counter +1);
```

2. 함수 할당 : setCounter( counter => counter +1 ) 

```
setCounter((current) => current+1)
```

- 함수의 첫번째 인자 : 현재 값
- 함수의 return 값 : 새로운 값
