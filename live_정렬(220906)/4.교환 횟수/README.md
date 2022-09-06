나의 풀이

```js
const solution = (nums) => {
  let n = nums.length
  let answer = Array(n).fill(0)
  let tempArr = [...nums]
  for (let i = 0; i < n - 1; i++) {
    let minI = i
    for (let j = i + 1; j < n; j++) {
      if (tempArr[j] < tempArr[minI]) {
        minI = j
      }
    }
    if(minI !== i) {
      [tempArr[i], tempArr[minI]] = [tempArr[minI], tempArr[i]]
      answer[minI]++
      answer[i]++
    }
  }
  return answer;
}
```

강사님의 풀이

```js

```

FEEDBACK
