# geolocation

## navigator
- 함수를 이용해 사용자의 위치를 알아냄
```
navigator.geolocation.getCurrentPosition(onGeoOk,onGeoError);
```
- 2개의 인자 필요 
- 1st => 성공했을 경우 실행될 함수
- 2nd => 실패했을 경우 실행될 함수

## position
> JS는 user의 위치를 전달해줌

![image](https://user-images.githubusercontent.com/90364684/211210936-23dbac24-45a8-4981-9012-c35299623247.png)

- position.coords.latitude : 위도 
- position.coords.longitue : 경도

