# x만큼 간격있는 n개의 숫자

# 문제설명


    문제 설명
    함수 solution은 정수 x와 자연수 n을 입력 받아, x부터 시작해 x씩 증가하는 숫자를 n개 지니는 리스트를 리턴해야 합니다. 다음 제한 조건을 보고, 조건을 만족하는 함수, solution을 완성해주세요.

    제한 조건
    x는 -10000000 이상, 10000000 이하인 정수입니다.
    n은 1000 이하인 자연수입니다.
    입출력 예
    x	n	answer
    2	5	[2,4,6,8,10]
    4	3	[4,8,12]
    -4	2	[-4, -8]


## 내가 쓴 코드
```javascript
function solution(x, n) {
    var answer = [];
    var d=0;
    for(let i=0; i<n; i++){
        d=d+x;
        answer[i]=d;
    }
    return answer;
}

```

## 다른 사람이 쓴 코드


```javascript
function solution(x, n) {
    var answer = [];
    for (let i = 1; i <= n; i++) {
        answer.push(x*i)
    }
    return answer;
}
```
+ `push`: 배열에 추가하는거



```javascript
function solution(x, n) {
    return Array(n).fill(x).map((v, i) => (i + 1) * v)
}
```
순서

1. 빈 배열을 생성한다. --> Array
2. 빈 배열을 x로 채운다. --> fill
3. 1부터 n까지의 값이 x와 곱해져 return 한다.


+ `Array`: 배열을 생성할떄 사용
+ `fill`: 배열안을 채워줄 때 쓰는거
+ `map`: 


### .map((v, i) => (i + 1) * v) 코드에 대하 설명

1. map을 사용하여 배열의 각 요소를 `(i + 1) * x`로 변환한다.

2. i는 배열의 인덱스이므로, i + 1을 곱하면 `1부터 n까지의 값이 x와 곱해진 형태`가 된다.

3. v는 fill(x)로 인해 모든 요소가 x이므로 `(i + 1) * v` ==`(i + 1) * x`