
## Mumbling

This time no story, no theory. The examples below show you how to write function `accum`:



## Example:

```javascript
accum("abcd") -> "A-Bb-Ccc-Dddd"
accum("RqaEzty") -> "R-Qq-Aaa-Eeee-Zzzzz-Tttttt-Yyyyyyy"
accum("cwAt") -> "C-Ww-Aaa-Tttt"
```


## Solution:

```javascript
function accum(s) {
    let arr = Array.from(s);
    return arr.map((item, id) => item[0].toUpperCase() + item.toLowerCase().repeat(id)).join('-');
}
```


