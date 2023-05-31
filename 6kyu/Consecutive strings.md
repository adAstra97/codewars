
## Consecutive strings
You are given an array(list) strarr of strings and an integer k. Your task is to return the first longest string consisting of k consecutive strings taken in the array.

n being the length of the string array, if `n = 0` or `k > n` or `k <= 0` return "" (return `Nothing` in Elm, "nothing" in Erlang).





## Solution:

```javascript
function longestConsec(strarr, k) {
   if (strarr.length == 0 || k > strarr.length || k <= 0){
      return '';
   } else {
      let arr =[];
      for (let i = 0; i < strarr.length; i++) {
         arr[i] = strarr.slice(i, k + i).join('');
      }
      return arr.find(item => item.length === (Math.max(...arr.map(item => item.length))));
   }
}
```


