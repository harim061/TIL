# filter
> 걸러주는 역할

```
const arr = [1234,5454,223,122,45,6677]

function Filter(item) {return item > 1000 }
```
![image](https://user-images.githubusercontent.com/90364684/211209898-8259ea3f-1a6f-4c50-b1cb-f4f5dd291de0.png)

- 1000이 넘는 item 값은 true 반환 => 배열에 유지
- 1000이 넘지않는 item 값은 false 반환 => 배열에서 삭제

![image](https://user-images.githubusercontent.com/90364684/211210006-4e3d7bd0-c7e6-452d-a33c-1c0a3ce4b9eb.png)

- false가 return 될 경우 배열에서 삭제

![image](https://user-images.githubusercontent.com/90364684/211210028-b4009b46-89e9-429d-aadf-a7e3c7ad35d2.png)

- 3이랑 같을 경우는 false이므로 3 삭제
