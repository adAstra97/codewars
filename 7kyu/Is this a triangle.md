
## Is this a triangle?


Implement a function that accepts 3 integer values a, b, c. The function should return true if a triangle can be built with the sides of given length and false in any other case.


## Solution:

```javascript
function isTriangle(a,b,c) {
  if (c < (a + b) && a < (b + c) && b < (c + a) ) {
    return true;
  } else {
    return false;
  }
}
```


