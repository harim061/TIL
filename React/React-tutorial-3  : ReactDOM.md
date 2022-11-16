# 3. ReactDOM
## 3-1. ReactDOM Intro
> ReactDOM is the glue between React and the DOM

- React creates a Virtual DOM, then ReactDOM is the library that efficiently updates the DOM based on that Virtual DOM

- 실제 돔을 메모리에 복사해준 것
- 데이터가 바뀌면 가상돔에 렌더링 > 이전 가상돔과 비교 > 실제 돔에 바뀐 부분만 적용
- ReactDOM receives those instructions from React and then efficiently updates the DOM

### Why is it a separate library?
- React and ReactDOM were part of the same library called React
- got split into two seperate libraries, to allow for the launch of React Native.

#### React Native
> React Native is the glue between React and native apps.

- React Native is outsdie the scope of this course
- React is the library that lets you write reusable UI and then
    - ReactDOM makes this UI visible in the browser
    - React Native makes this UI visible in a native app
    
🔸 React library has nothing to do with a web browser
- ReactDOM = idea of React + web browser
- React Native = ideo of React + native app

❓ Native App : Android ios 같은 어떤 구체적인 플랫폼만을 위해 만들어진 응용 프로그램. 흔히 말하는 '어플리케이션'

### Reconciliation
> 재조정(reconciliation) : 바뀐 부분만 실제 돔에 적용시켜주는 것

## 3-2. ReactDOM Usage
```
npm install react-dom
npm install react react-dom
```
### importing
```
import {createRoot} from "react-dom/client";
```

### Root of your app
- we use ReactDOM to render our React Elements on the page
- you have to tell ReactDOM where to render these elements
> root

```
<div id="root"></div>
```

#### *createRoot().render()* method
```
import {createRoot} from "react-dom/client";

const root = document.querySelector("#root");
createRoot(root).render(React.createElement("p", {}, "Hello World"));
```
- createRoot().render() method from ReactDOM receives a React Element and them makes it visible in the actual DOM

1. (querySelector 또는 getElementById 사용) 루트 요소에 대한 참조를 가져옴
2. createRoot(root)를 이용하여 React 앱의 루트 생성
3. .render()를 호출하고 React 요소로 전달

## 3-3. Root Element

> *root* element that pass to ReactDOM will become completely managed by React
>
> should not write any kind of JS that changes its content

### Use cases
1. Apps built with React
	- usually has a single root element
    - the whole application is rendered inside that root element
    
2. Integrate React into an existing App
	- integrate React to make a certain part of that website interactive


👻
- React JS : 라이브러리
- React DOM : element들을 html body에 둘 수 있도록 해줌
- ReactDOM.render(element, element 위치) : element를 가지고 HTML로 만들어 배치하겠다. 사용자에게 보여주겠다


