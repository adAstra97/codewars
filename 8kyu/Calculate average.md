
## Calculate average

Write a function which calculates the average of the numbers in a given list.

**Note:** Empty arrays should return 0.



## Solution:

```javascript
function findAverage(array) {
  if (array.length > 0) {
    return array.reduce((acc, item) => acc + item, 0)/array.length;
  }
  return 0;
}
```


