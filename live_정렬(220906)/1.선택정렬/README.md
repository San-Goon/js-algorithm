나의 풀이

```js
const solution = (nums) => {
  let answer = [...nums]
  for (let i = 0; i < answer.length - 1; i++) {
    let minI = i
    for (let j = i + 1; j < answer.length; j++) {
      if (answer[j] < answer[minI]) {
        minI = j
      }
    }
    if(minI !== i) {
      [answer[i], answer[minI]] = [answer[minI], answer[i]]
    }
  }
  return answer;
}
```

강사님의 풀이

```js

```

FEEDBACK
[answer[i], answer[minI]] = [answer[minI], answer[i]] 배열요소 교체방법에 주목하자!
