# Props

> 첫 번째이자 유일한 인자

> 부모에서 자식으로 데이터를 넘길 때 사용하는 argument의 역할

💥 같은 스타일을 모두 갖는 단 한가지의 컴포넌트로 만들어 재사용을 할 수 없을까?

💡 여러 버튼을 복사 붙여넣기 하는 대신에 어떤 prop들을 받을 수 있는 Btn 컴포넌트를 만들기

보통 이 인자를 props라고 부름 👉 컴포넌트에 데이터를 보내기위한 

```
function Btn(props){    //Btn 컴포넌트
            return (
                <button
                    style={{
                        backgroundColor:"tomato",
                        color:"white",
                        padding:"10px 20px",
                        border : 0,
                        borderRadius : 10,
                        
                    }}    
                >{props.text}</button>
            )
        }

function App(){
    return (
        <div>
            <Btn text="hi"/> //text prop
            <Btn text="bye"/>
        </div>
    )
};
        
```
- props는 객체
- 키를 가져와 사용 가능

💡 Btn 컴포넌트가 prop에 접근할 수 있는 방법 : 컴포넌트들은 괄호에 첫 번째 인자로 prop들을 하나의  받음

```
function Btn({text){
            return (
                <button
                    style={{
                        backgroundColor:"tomato",
                        color:"white",
                        padding:"10px 20px",
                        border : 0,
                        borderRadius : 10,
                        
                    }}    
                >{text}</button>
            )
        }
        
```
### props로 함수 넘겨주기
![image](https://user-images.githubusercontent.com/90364684/212730342-0234f8e2-f800-4e58-8bb3-d8a6e4f85875.png)

-> 이벤트 리스너 아님, props

-> onClick은 단순히 prop

💡props에 무언가를 넣을 때 자동적으로 return에 들어가지 않음 -> 직접 써야함

## Memo
> props가 변경되지 않을 때 다시 그릴 필요가 없다는 것을 말해줌

> 많은 양의 자식 컴포넌트를 가지고 있을 때 사용하면 좋음

![image](https://user-images.githubusercontent.com/90364684/212743416-1f7b8a4c-40f0-4f79-b383-22c8fbc2705f.png)

![image](https://user-images.githubusercontent.com/90364684/212743448-1865e317-24ab-4a8a-a183-027bf3769db1.png)

- props가 바뀌지 않는 부분까지 렌더링 됨

![image](https://user-images.githubusercontent.com/90364684/212743601-89faadd4-73db-4c14-89b3-cac16b3f68aa.png)

```
 const MemorizedBtn = React.memo(Btn)
```

![image](https://user-images.githubusercontent.com/90364684/212743655-dcec0c3e-37bd-4293-bbea-40bf61a1999e.png)

- props가 바뀐 부분만 렌더링
 
## props type
 
> 잘못된 props를 전달할 수 있음

💡 어떤 타입의 prop을 받고 있는지 체크해줌

```
component.propTypes ={
   propName : propTypes     
}
```

![image](https://user-images.githubusercontent.com/90364684/213488443-a628e752-23da-4b44-8580-328f8a645c55.png)

### PropTypes.type.isRequired

> 필수 
```
component.propTypes ={
   propName : propTypes.type.isRequired
}
```
![image](https://user-images.githubusercontent.com/90364684/213489281-26ee02da-2ed6-46fe-ba03-6820fd681ff4.png)

```
 function Btn({text,fontSize = 14})
```
- js 이용하여 기본값을 줄 수도 있음



