# JSX

> 자바스크립트를 확장한 문법

```
const btn2 = React.createElement("button",{
onClick :()=>console.log("im clicked"),
  style:{
    backgroundColor:"tomato",
        }
  },"Click me");
```

- createElement 사용 ❌
```
const btn  =(
    <button
      style={{backgroundColor:"tomato",}}
      onClick={() => console.log("im click")}
    />
);
```

- 보통의 HTML과 비슷
- property를 HTML태그 속성처럼 적음

- 항상 대문자 컴포넌트 사용

### < Button /> vs < button />
```
const Container =()=>(
  <div>
      <Title />
      <Button /> //내가 만든 컴포넌트
      <button /> //html 버튼
  </div> );
```


1) arrow function
```
const Title =()=>(
  <h3 id="title" onMouseEnter={() => console.log("mounse enter")}>
    Hello
  </h3>
  );
``` 

2)
```
function Title(){
  return (
   <h3 id="title" onMouseEnter={() => console.log("mounse enter")}>
    Hello
   </h3>
   );
};
```

       
  
