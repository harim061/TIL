# Router

> URL에 따라 알맞는 페이지 전환
>
> 페이지별로 컴포넌트들을 분리해가며 프로젝트를 관리
>
> App.js 는 router를 render, router는 URL을 보고있는 컴포넌트

## 라우터 적용하기
```
npm i react-router-dom
```

``` 
//App.js

import{
    BrowserRouter as Router,
    Routes,
    Route
} from "react-router-dom";
```

1. 페이지 컴포넌트 만들기


![image](https://user-images.githubusercontent.com/90364684/213871572-5a5187b1-457b-4155-9a94-3a59270f3473.png)

- 보여지게 될 페이지 컴포넌트 생성

2. Route 컴포넌트로 경로에 컴포넌트 넣기
```
function App(){
    return (
    <Router>
        <Routes>
            <Route path='/' element={<Home/>}/>
            <Route path='/movie' element={<Detail/>}/>
        </Routes>
    </Router>
    )
    
};
```
- Route 컴포넌트는 Routes 컴포넌트 내부에서 사용

```
<Route path="주소" element={보여줄 컴포넌트 } />
```

3. Link 컴포넌트 사용하여 다른 페이지로 이동하기
```
<Link to="경로"> </Link>
```

## 다이나믹 url 적용하기

```
<Route path='/movie/:id' element={<Detail/>}/>
```
`/movie/:id` 로 줘야함 `movie/id`는 텍스트 그대로 이므로

```
<Link to={`/movie/${id}`}>
```
![image](https://user-images.githubusercontent.com/90364684/213872239-5d735d59-bab0-4c3f-8c1a-988896457c94.png)

## useParams

> urls에 있는 값을 반환해주는 함수

`<Route path='/movie/:id' element={<Detail/>}/>` url에는 id가 들어갈 자리가 있음

```
//Detail.js

import { useParams } from "react-router-dom";

function Detail(){

    const x = useParams()

    console.log(x);
    
    return(
    <h1>detail</h1>
    )
}

export default Detail;
```
- useParams를 이용하여 url에 있는 id값 가져오기

![image](https://user-images.githubusercontent.com/90364684/213872557-0f1c783d-d217-4029-8e36-85d7f603aef4.png)

