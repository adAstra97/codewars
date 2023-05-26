
## Reversed sequence

Build a function that returns an array of integers from n to 1 where `n>0`.

## Example:

```javascript
`n=5` --> `[5,4,3,2,1]`
```

## Solution:

```javascript
const reverseSeq = n => {
  let arr = [];
  for (let i = 1; i <= n; i++) {
    arr.unshift(i);
  }
  return arr;
}
```


