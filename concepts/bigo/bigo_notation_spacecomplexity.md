[BigO](/links/bigO.md)
[PrevRead](./bigo_notation_timecomplexity.md)

## Space Complexity

Using BigO notation to define how space used by algorithm changes with input n.
We ignore space taken by the inputs

## Rules of thumb

- Most Primitive (Boolean, Numbers, undefined, null) are constant space.
- String require O(n) space where n is the string length
- Reference types are also O(n) where n is lenght of array or number of keys for
  object.
  
## Example

```js
function addUpTo(n) {
    let total = 0;        // 1 variable
    for (let i =1; i<=n; i++) {  // second variable
        total +=i;              
    }
    return total;
}```

- With increase in N, we should only even have 2 variables.
- the space complexity is equalt to 0(1)



