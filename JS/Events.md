# Events

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

## window.InnerWidth
```
var intViewportWidth = window.innerWidth;
```
> 뷰포트의 폭을 받아올 수 있음

## path
❓button을 클릭했을 때 어떤 button인지 모르는 경우가 있음

💡event는 property를 가지는데 어떤 button이 클린 되어있는지 알려줌
```
const li = event.target.parentElement;
```
- target :  해당 객체를 지정
- parentElement : 해당 객체의 부모
