
## Replace With Alphabet Position
In this kata you are required to, given a string, replace every letter with its position in the alphabet.

If anything in the text isn't a letter, ignore it and don't return it.



## Solution:

```javascript
function alphabetPosition(text) {
   let alfabet = [];
   let arrFromStr = text.toLowerCase().split('');
   let result = [];
   for (let i = 97; i <= 122; i++) {
      alfabet.push(String.fromCharCode(i));
   }
   for (let i = 0; i < arrFromStr.length; i++) {
      let index = alfabet.indexOf(arrFromStr[i]);
      if (index !== -1) {
         result.push(index + 1);
      } else {
         continue;
      }
   }
   return result.join(' ');
}
```


