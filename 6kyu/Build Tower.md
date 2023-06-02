
## Build Tower
Build a pyramid-shaped tower, as an array/list of strings, given a positive integer `number of floors`. A tower block is represented with `"*"` character.




## Solution:

```javascript
function towerBuilder(nFloors) {
   let array = [];
   for (let i = 0; i < nFloors; i++) {
      array.push(' '.repeat(nFloors - i - 1) + '*'.repeat(2 * i + 1) + ' '.repeat(nFloors - i - 1));
   }
   return array;
}
```


