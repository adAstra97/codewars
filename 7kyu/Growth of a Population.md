
## Growth of a Population
In a small town the population is `p0 = 1000` at the beginning of a year. The population regularly increases by `2 percent` per year and moreover `50` new inhabitants per year come to live in the town. How many years does the town need to see its population greater or equal to `p = 1200` inhabitants?

The function `nb_year` should return `n` number of entire years needed to get a population greater or equal to `p`.

`aug` is an integer, `percent` a positive or null floating number, `p0` and `p` are positive integers (> 0)






## Solution:

```javascript
function nbYear(p0, percent, aug, p) {
   let sum = 0;
   let count = 0;

   while (sum < p) {
      sum = Math.floor(p0 + p0 * percent/100 + aug);
      count ++;
      p0 = sum;
   }

   return count;
}
```


