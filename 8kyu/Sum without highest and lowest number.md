
## Sum without highest and lowest number

Sum all the numbers of a given array ( cq. list ), except the highest and the lowest element ( by value, not by index! ).

The highest or lowest element respectively is a single element at each edge, even if there are more than one with the same value.

Mind the input validation.


## Example:

```javascript
{ 6, 2, 1, 8, 10 } => 16
{ 1, 1, 11, 2, 3 } => 6
```

## Solution:

```javascript
function sumArray(array) {
  if (array == null) {
   return 0;
   } else {
   let indexMin = array.indexOf(Math.min(...array));
   let indexMax = array.indexOf(Math.max(...array));
   delete array[indexMin];
   delete array[indexMax];
   return summary = array.reduce((sum, current) => sum + current, 0);
  }
}
```


