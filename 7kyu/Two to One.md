
## Two to One


Take 2 strings `s1` and `s2` including only letters from `a` to `z`. Return a new sorted string, the longest possible, containing distinct letters - each taken only once - coming from s1 or s2.


## Example:

```javascript
a = "xyaabbbccccdefww"
b = "xxxxyyyyabklmopq"
longest(a, b) -> "abcdefklmopqwxy"

a = "abcdefghijklmnopqrstuvwxyz"
longest(a, a) -> "abcdefghijklmnopqrstuvwxyz"
```

## Solution:

```javascript
function longest(s1, s2) {
	let arr = Array.from(s1.concat(s2));
	let result = [];
	for (let i = 0; i < arr.length; i++) {
		if (!result.includes(arr[i])) {
			result.push(arr[i]);
		}
	}
	return result.sort().join('');
}
```


