# styleModule

- 컴포넌트 당 1개의 js 파일을 가질 수 있음


![image](https://user-images.githubusercontent.com/90364684/213511817-cf281812-8535-4df5-9cc1-196c537e7c0d.png)

- 컴포넌트 스타일은 .module.css 파일 생성 + import


![image](https://user-images.githubusercontent.com/90364684/213511943-b7b5275c-143d-4ab4-b2b9-714c4caffbf5.png)

![image](https://user-images.githubusercontent.com/90364684/213511983-f9210e50-cbce-4823-9ebc-219e1fa78670.png)

- className, id로 import한 스타일 객체 사용 및 전달
```
<button className={styles.btn}> </button>
```
- react 컴파일 과정 중 랜덤으로 class, id 생상됨

![image](https://user-images.githubusercontent.com/90364684/213512533-16008530-6dbf-4db0-a836-484e7fe81ad4.png)
