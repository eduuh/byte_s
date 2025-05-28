# Objects

## When to use Object

- When yu don't need ordering
- When you need fast access / insertion and removal.

## Big O of Objects

- Insertion - 0(1)
- Removal - 0(1)
- Searching - 0(N)
- Accessing - 0(1)

```js
let instructor = {
    firstName: "kelly",
    isInstructor: true,
    favoriteNumber: [1,2,3,4]
}
```
## Big O of Objects Methods

- Object.keys - 0(n)
- Object.values - 0(N)
- Object.entries - 0(N)
- hasOwnProperty - 0(1)

# Arrays

- Ordered lists but the order cames at a cost for some of the operations
(insertion & removal)
- access with index is 0(1) operation

## Methods

- Insertion (end) - push - 0(1)
- Insertion (begining) & Removing form begining  - 0(n)
   - we need re-index all other elements.
- Searching - 0(N)
- Accessing - 0(1)

### Array methods

- push - 0(1)
- pop - 0(1)
- shift - 0(N)
- unshift - 0(N)
- concat - 0(n)
- slice - O(n)
- splice - 0(n)
- sort - 0(n)
- forEach/map/filter/reduce/etc. - 0(n)
