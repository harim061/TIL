# React element

- react js 는 interactive하도록 만들어주는 라이브러리
- react-dom React element들을 html body에 두게 하는 라이브러리, 패키지 

## ReactDOM.render()
- render : React element를 가지고 html로 만들어 배치한다는 의미
- show it to the users
```
ReactDOM.render(span,root);
```
- span을 root안에 배치해라

```
const span =React.createElement("span",{ property }, "content"); 
```
- property : className, id, style, eventListener

![image](https://user-images.githubusercontent.com/90364684/210610795-24bbd538-9a24-4f62-afe2-cd07e4dfb978.png) 👉 ![image](https://user-images.githubusercontent.com/90364684/210610902-a2706b82-54cc-4eff-9ded-757c018b86e8.png)

💡React js : js -> html 

### container 만들어서 배치
```
const container = React.createElement("div",null,[span,button]);
```
- 배열 만들어서 span, button 함께 배치 가능

### property에 eventListener 달기
![image](https://user-images.githubusercontent.com/90364684/210612690-bffc4e7d-c7b4-4b53-abb2-5bbb0dd5dfac.png)
- js : click
- React js : onClick = on + event
