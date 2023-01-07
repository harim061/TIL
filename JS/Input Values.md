# Input Values

```
const loginForm = document.querySelector("#login-form");
const loginInput = loginForm.querySelector("input");

const loginInput2 = document.querySelector("login-form input");
```
### input의 내용 가져오기
> value 값 가져오기

### input의 유효성 검사 작동
> form 태그 사용

### 브라우저의 새로고침 막기
> preventDefault();

- form을 submit 하면 기본적오르 페이지를 새로고침
- preventDefault()함수를 사용하여 마금

```

function onLoginSubmit(event){
    event.preventDefault();
};
```
- addEventListener 안에 있는 함수는 직접 실행 x
- 브라우저가 실행, 해당 이벤트에 대한 정보 object을 갖는 것
- 해당 이벤트가 가진 기본 Default값을 발생 시키지 않는 것 -> preventDefault는




