
## Highest Scoring Word

Given a string of words, you need to find the highest scoring word.

Each letter of a word scores points according to its position in the alphabet: `a = 1, b = 2, c = 3` etc.

For example, the score of `abad` is `8` (1 + 2 + 1 + 4).

You need to return the highest scoring word as a string.

If two words score the same, return the word that appears earliest in the original string.

All letters will be lowercase and all inputs will be valid.




## Solution:

```javascript
function high(x){
   let alphabet = {
      A: 1, B: 2, C: 3, D: 4, E: 5, F: 6,
      G: 7, H: 8, I: 9, J: 10, K: 11, L: 12,
      M: 13, N: 14, O: 15, P: 16, Q: 17, R: 18,
      S: 19, T: 20, U: 21, V: 22, W: 23, X: 24,
      Y: 25, Z: 26,
   };
   let arr = x.toUpperCase().split('');
   let sum = 0;
   let result = [];
   for (let i = 0; i < arr.length; i++) {
      arr[i] = alphabet[arr[i]];
      if (arr[i] !== undefined) {
         sum += arr[i];
         if (i === arr.length - 1) {
            result.push(sum);
         }
      } else {
         result.push(sum);
         sum = 0;
      }
   }
   let index = result.indexOf(Math.max(...result));
   return x.split(' ')[index];
}
```


