
## Equal Sides Of An Array

You are going to be given an array of integers. Your job is to take that array and find an index N where the sum of the integers to the left of N is equal to the sum of the integers to the right of N. If there is no index that would make this happen, return `-1`.

## Solution:

```javascript
function findEvenIndex(arr) {
let sum1;
let sum2;

for (let i = 0; i < arr.length; i++) {
   sum1 = arr.slice(0, i).reduce((sum, item) => sum + item, 0);
   sum2 = arr.slice(i+1, arr.length).reduce((sum, item) => sum + item, 0);
   if (sum1 === sum2) {
      return i;
   }
}
return -1;
}
```


