
## Tribonacci Sequence
As the name may already reveal, it works basically like a Fibonacci, but summing the last 3 (instead of 2) numbers of the sequence to generate the next.

Signature will always contain 3 numbers; n will always be a non-negative number; if `n == 0`, then return an empty array (except in C return NULL) and be ready for anything else which is not clearly specified ;)





## Solution:

```javascript
function tribonacci(signature,n) {
   for (let i = 3; i < n; i++) {
      signature.push(signature[i - 3] + signature[i - 2] + signature[i - 1]);
   }
   return signature.splice(0, n);
}
```


