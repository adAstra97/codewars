
## Fake Binary


Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the resulting string.

## Solution:

```javascript
let fakeBin = x => Array.from(x).map(x => (x < 5) ? 0 : 1).join('');
```


