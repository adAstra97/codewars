
## Duplicate Encoder
The goal of this exercise is to convert a string to a new string where each character in the new string is "(" if that character appears only once in the original string, or ")" if that character appears more than once in the original string. Ignore capitalization when determining if a character is a duplicate.




## Solution:

```javascript
function duplicateEncode(word){
   let arr = word.toLowerCase().split('');
   let result = [];
   for (let i = 0; i < arr.length; i++) {
      if (arr.indexOf(arr[i]) === arr.lastIndexOf(arr[i])) {
         result.push('(');
      } else {
         result.push(')');
      }
   }
   return result.join('');
}
```


