
## The Supermarket Queue
There is a queue for the self-checkout tills at the supermarket. Your task is write a function to calculate the total time required for all the customers to check out!




## Solution:

```javascript
function queueTime(customers, n) {
   let cashboxes = [...Array(n)].fill(0);

   customers.forEach(el => {
      cashboxes[cashboxes.indexOf(Math.min(...cashboxes))] += el;
   });

   return Math.max(...cashboxes);
}
```


