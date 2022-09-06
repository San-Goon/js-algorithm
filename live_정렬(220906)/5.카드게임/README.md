나의 풀이

```js
const solution = (nums,k) => {
    let answer = 0;
    let tempArr = [...nums]
    let n = nums.length
    let diff = []
    tempArr.sort((a,b) => b-a)
    for (let i = 0; i < n; i += 2) {
        answer += tempArr[i + 1]
        diff.push(tempArr[i] - tempArr[i+1])
    }
    diff.sort((a,b) => b-a)
    for (let i = 0; i < k; i++) {
        answer += diff[i]
    }
    return answer
}
```

강사님의 풀이

```js

```

FEEDBACK
