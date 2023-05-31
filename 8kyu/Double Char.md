
## Double Char
Given a string, you have to return a string in which each character (case-sensitive) is repeated once.







## Solution:

```javascript
let doubleChar = str => Array.from(str).map(item => item + item).join('');

```


