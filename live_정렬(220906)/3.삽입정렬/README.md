나의 풀이

```js
const solution = (nums) => {
  let answer = [...nums]
  let n = answer.length
  for (let i = 1; i < n; i++) {
    let tmp = answer[i]
    let j = i - 1
    for (j; j >= 0; j--) {
      if (answer[j] > tmp) answer[j + 1] = answer[j]
      else break
    }
    answer[j + 1] = tmp
  }
  return answer;
}
```

강사님의 풀이

```js

```

FEEDBACK
