# Effect
> 우리 코드가 딱 한 번만 실행하도록 해줌

> 코드의 실행 시점을 관리할 수 있는 선택권을 얻음


💥 state가 변하면 리렌더링 됨. 만약 리렌더링을 시키고 싶지 않다면? (api 재호출)

💡 useEffect

### argument 
1. 우리가 딱 한번만 실행하고 싶은 코드
2. [ ] 변화할 때 코드가 실행할 것이라고 알려주는 부분

![image](https://user-images.githubusercontent.com/90364684/213519156-336cb5f7-5164-4109-9b9d-ea865b02582f.png)

![image](https://user-images.githubusercontent.com/90364684/213519181-e7b1e4a7-a06b-4d45-83be-1136c7312189.png)

- useEffect 안의 함수는 한 번만 호출

💥 내 코드의 특정 부분만이 변화할 때 원하는 코드들을 실행할 수 있는 방법은?
```
const [counter,setValue] = useState(0);
  const [keyword, setKeyword] = useState("");

  const onClick =()=>{
    setValue((prev) =>prev +1)
  }
  console.log("i run all the time");

  useEffect(()=>{
    console.log("called api");
  },[]);

  console.log("search for");
  
  const onChange =(event)=>{
    setKeyword(event.target.value);
  }
```

![image](https://user-images.githubusercontent.com/90364684/213521924-f725efd3-db8e-4558-865c-270b11d24c57.png)

- onClick이 실행 될 때 console.log("search for")도 실행됨

```
  useEffect(()=>{
    console.log("search for",keyword);
  },[keyword]);
```
 
![image](https://user-images.githubusercontent.com/90364684/213522441-f97223c1-e89c-4c16-83ff-8464d7b01b58.png)

- keyword가 바뀌는 경우에만 실행됨

```
useEffect(()=>{
  console.log("keyword counter");
  }
 },[keyword,counter]);
```
- 두개도 가능 
