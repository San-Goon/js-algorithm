나의 풀이

```js
const solution = (nums) => {
  let answer = [...nums]
  for (let i = 0; i < answer.length - 1; i++) {
    for (let j = 0; j < answer.length - 1 - i; j++) {
      if (answer[j] > answer[j + 1]) {
        [answer[j], answer[j + 1]] = [answer[j + 1], answer[j]]
      }
    }
  }
  return answer;
}
```

강사님의 풀이

```js
const solution = (nums) => {
    let n = nums.length;
    for (let i = 0; i < n - 1; i++) {
        for (let j = 0; j < n - i - 1; j++) {
            if (nums[j] > nums[j + 1]) {
                [nums[j], nums[j + 1]] = [nums[j + 1], nums[j]]
            }
        }
    }
    return nums;
}
```

FEEDBACK
