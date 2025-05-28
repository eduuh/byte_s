<!--toc:start-->
- [What's the idea here?](#whats-the-idea-here)
- [Example](#example)
- [Who cares?](#who-cares)
  - [Lets compare some functions](#lets-compare-some-functions)
- [Faster](#faster)
  - [Timing Function](#timing-function)
    - [Problem with Time](#problem-with-time)
  - [Count number of simple operations](#count-number-of-simple-operations)
<!--toc:end-->

[bigO](../../links/bigO.md)

## What's the idea here?

Imagine we have multiple implementation of the same functions

How do we know what best? that what bigO is about.

## Example

> Write a function that accepts a string input and returns a reversed copy?

You can have more than 10 implementation of the problem.

Can we have a numeric representation of best solutions.

## Who cares?

1. The level of care depends on the need.
   - less important: this could be interview.
   - this could be optimizations.
   
2. it's important to have a precise vocabulary to talk about how our code performs.
3. Useful for discussing trade-offs between different approaches.
4. When your code slows down or crashes, identifying parts of the code that are
   inefficent can help us find pain points in our applications.

### Lets compare some functions

> suppose we want to write a function that calculates the sum of all numbers
> from 1 up to (and including) some number n.

Solution 1

```js
function addUpTo(n) {
    let total = 0;      //accumulator
    for (let i =1; i<=1; i++) {
        total +=i;
    }
    return total;
}
```


Solution 2

```js
funtion addUpTo(n) {
    return n* (n+1) / 2
}

```
- This are two solutions but which is better?
   - is better faster? Less memory-intensive? more readable?

## Faster

### Timing Function

- Simplest way to test is to use timing functions
    Solution1: 1.25s
    Solution2: 0.002s
   
   - But this varies

#### Problem with Time

- Different machine will record different times.
- The same machine will record different times.
- For fast algorithms, speed measurements may not be precise enough.

### Count number of simple operations

- Rather that counting seconds, which are so variable.
- We count the `number of simple` operations that computer has to perform.


```js
function addUpTo(n) {
    return n * (n + 1) / 2; // 1 multiplication 1 addition 1 division
}
```
- Total number of operations are; 3

```js
function addUpTo(n) {
    let total = 0;      //1 assignment 
    for (let i =1; i<=n; i++) { //1 assignment, n 
        total +=i;              // n addition n assignments 2n
    }
    return total;
}
```
- Counting all operation can be hard!
   - it does not mater. We focus on the big picture.
   - we are looking at the tread
   
- When n grow larger the number of comparison grows


[Next Read](./bigo_notation_timecomplexity.md)
