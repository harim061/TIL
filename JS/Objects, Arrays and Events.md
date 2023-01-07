# Objects, Arrays and Events

## contextmenu event
> 마우스 우 클릭시 생기는 이벤트
```
window.addEventListener("contextmenu",handleMouseRightClick);
```
## superEventHandler
> 객체 안에 함수 저장하기
```
const Student = {
  name = "harim",
  age = 21,
  sayName : function(){
    alert(`my name is ${this.name[0]}`);
    }
 };
 ```
 function name : function(){
    }
방식으로 객체 안에 function 저장 가능
