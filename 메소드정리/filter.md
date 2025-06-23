# filter

목적:조건을 만족하는 요소만 걸러내는 함수
ex)배열에서 짝수인경우만 찾는경우

약간 if문이랑 비슷하다고 생각한다.

# 사용법
```ts
array.filter(element => 조건)
```

# 예제
```ts
let array = [3,5,11,0,9,'string'];
let result = array.filter((value) => value < 10)
console.log(result);
```
10보다 작은것을 찾는다.


### filter안에있는것은 꼭 value이어야할까?

아니다. value말고도 `value, item, element`도 가능하다.