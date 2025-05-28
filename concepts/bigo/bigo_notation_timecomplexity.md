[BigO](../../links/bigO.md)
[Prev Read](./bigO_introduction.md)

# Big O

Big O notation is way of formalizing fuzzy counting.

It allows us to talk formally about how the runtime of alorithm grows as the
input grows

BigO focus on the worst case scenarios

## Notation vs Comparisons

n =     1   2    3    4    5   

O(1):   ●    ●    ●    ●    ●  
O(log): ●    ●●   ●●   ●●●  ●●● 
O(n):   ●    ●●   ●●●  ●●●● ●●●●●
O(n²):  ●    ●●●  ●●●●●  ●●●●●●●●

## 🔍 Visual Metaphor

Each "thread" shows how much work increases as n increases.

O(1) stays flat.

O(log n) grows very slowly.

O(n) grows proportionally.

O(n²) and O(2ⁿ) blow up fast — like exploding threads.

## Examples

## Big O(1)

```js
function addUpTo(n) {
    return n * (n + 1) / 2; // 1 multiplication 1 addition 1 division
}

//total operations: 3
```

## Big 0(n)

```js
function addUpTo(n) {
    let total = 0;      //1 assignment 
    for (let i =1; i<=n; i++) { //1 assignment, n 
        total +=i;              // n addition n assignments 2n
    }
    return total;
}

```
Similary two loops is 0(n)

```js
function countUpAndDown(n) {
  // Count up from 1 to n
  for (let i = 1; i <= n; i++) {
    console.log(i);
  }

  // Count down from n - 1 to 1
  for (let i = n - 1; i >= 1; i--) {
    console.log(i);
  }
}

```
## O(n²) Nested Loops 

```js
function printAllPairs(n) {
  for (let i = 0; i < n; i++) {
    for (let j = 0; j < n; j++) {
      console.log(`(${i}, ${j})`);
    }
  }
}

```
## Simpflify big o notations rules

1. Constants do not matter
    O(2n) => 0(n)
    O(500) => 0(1)

2. Smaller Terms don't matter.
    O(13n²) => O(n²)
    O(1000n + 50) => O(n)
    O(n² + 5n + 1000) => O(n²)

## Big O Shorthands

- Analyzing complexity with big 0 things get complicated

1. Arithemetic operation are constant
2. Variable assignment is constant
3. Accessing elements in array or object using index or key is constant runtime
4. In loop, the complexity is the length of loop multiplied by what happens
   inside the loop.

### Some examples that might confuse.

- Always ask the question of what happens when n increases.

complexity is: 0(1) -> even with the loop

```js
function logAtMost5(n) {
  const limit = Math.min(n, 5);
  for (let i = 1; i <= limit; i++) {
    console.log(i);
  }
}

```

[NextRead](./bigo_notation_spacecomplexity.md)
