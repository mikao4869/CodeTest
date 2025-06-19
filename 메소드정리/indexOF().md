# inddexOF()

정의: 문자열에서 특정한 문자를 찾는거 

즉 리스트에서 있는 문자열의 위치의 값을 반환한다. 



```TS
const str = "abab";

document.writeln(str.indexOf('ab')); // 0
```

이거 값이 0인데, 

그 이유는 ab의 처음시작하는 배열의 값이 0이기 때문이다. 


# 규칙


**1. 인덱스는 0부터 시작함.**




**2. 못 찾으면 -1을 반환함.**

```ts
const str = "abab";
document.writeln(str.indexOf('abc')); // -1

```

abab는 abc가 없기 떄문에 -1을 반환함

**3. 시작위치 설정**
```ts
console.log(str.indexOf("o", 5)); // 👉 7
```
이 코드면 5부터 시작함

## 배열에서 indexOF

```ts
const arr = [1, 3, 5, 3, 9];
console.log(arr.indexOf(3)); // 
```
`찾고자 하는 숫자중에 가장 먼저 나온 인덱스 번호를 보여줌 `

즉 arr배열에서 3이라는 값을 찾는데
3이 여러개있지만 그중에서 `1번` 자리에있는 3이 가장 먼저 있기 때문에 값이 1임

# 사용법

```ts
if (arr.indexOf(value) !== -1) {
  // value가 있다
}

```

배열에서 값이 있는지 없는지 확인하는거

