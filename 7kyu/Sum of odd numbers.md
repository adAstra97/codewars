
## Sum of odd numbers

Given the triangle of consecutive odd numbers:

```javascript
             1
          3     5
       7     9    11
   13    15    17    19
21    23    25    27    29
...
```
Calculate the sum of the numbers in the `n` row of this triangle (starting at index 1) e.g.: (Input --> Output)


## Example:

```javascript
1 -->  1
2 --> 3 + 5 = 8
```

## Solution:

```javascript
function rowSumOddNumbers(n) {
	return Math.pow(n, 3);
}
```


