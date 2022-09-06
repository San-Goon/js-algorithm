나의 풀이

```js
const solution = (n) => {
  let answer = 0;
  let sum = 0;
  let lt = 1;
  for (let rt = 1; rt <= Math.ceil(n/2); rt++) {
    sum += rt;
    while (sum > n) {
      sum -= lt;
      lt++;
    }
    if (sum === n) answer++
  }
  return answer;
}
```

강사님의 풀이

```js

```

FEEDBACK
좋은 코드라고 칭찬을 주셨당!
