
## Remove exclamation marks
Write function RemoveExclamationMarks which removes all exclamation marks from a given string.





## Solution:

```javascript
let removeExclamationMarks = (s) => s.replace(/[^\w ]+/gi, '');

```


