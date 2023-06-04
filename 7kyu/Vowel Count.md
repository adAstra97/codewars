
## Vowel Count
Return the number (count) of vowels in the given string.





## Solution:

```javascript
function getCount(str) {
   let arr = str.split('');
   let count = 0;

   for (let i = 0; i < arr.length; i++) {
      arr[i] === 'a' || arr[i] === 'o' || arr[i] === 'e' || arr[i] === 'i' || arr[i] === 'u' ? count++ : count;
   }
   return count;
 }
```


