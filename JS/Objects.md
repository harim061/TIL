# Objects
> property를 가진 데이터를 저장함
> 
```
const player = {
    name : "harim",  
    points : 10,
};

console.log(player.name); //harim
console.log(player["name"]); //harim
```

❓const 수정 가능?
- object 안의 속성 변경 not modify object 
```
player.points = 20;
```
- when you try to update whole constant -> error
```
player = 20 ; //error
```
