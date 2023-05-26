
## Quarter of the year

Given a month as an integer from 1 to 12, return to which quarter of the year it belongs as an integer number.

For example: month 2 (February), is part of the first quarter; month 6 (June), is part of the second quarter; and month 11 (November), is part of the fourth quarter.
## Solution:

```javascript
const quarterOf = (month) => {
   return (12 / month <= 1.2) ? 4 :
          (12 / month < 2) ? 3 :
          (12 / month <= 3) ?  2 : 1;
}
```


