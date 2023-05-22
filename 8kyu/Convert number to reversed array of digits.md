
## Convert number to reversed array of digits

Given a random non-negative number, you have to return the digits of this number within an array in reverse order.


## Example:

```javascript
35231 => [1,3,2,5,3]
0 => [0]
```

## Solution:

```javascript
let digitize = n => Array.from(n.toString()).map(digit => +digit).reverse();
```


