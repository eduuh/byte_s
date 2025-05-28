[bigO](../../links/bigO.md)
[PrevRead](./bigo_notation_spacecomplexity.md)

## Logarithm

In reality complexities are not simple. 

Logarithm complexities appears more often that we migh want to accept.

Logarithm of a number rougly measures the number of times we can divide that
number by the base before you get a number less that that number or equal to
that number.

## complexity

- Algorithm with (log n) time complexity is great.
- Recursion contains logarithm space complexities


## Who cares

- certain algorithm contain log complexities 
- Efficient sorting algorithm involves logarithm


## 🧠 Common Logarithms in Programming

- **Base 10** → `Math.log10(x)`
- **Base 2** → `Math.log2(x)`
- **Natural log (base _e_ ≈ 2.718)** → `Math.log(x)`

```js
console.log(Math.log2(8));    // 3
console.log(Math.log10(100)); // 2
console.log(Math.log(1));     // 0 (natural log)


🚩 What is a Logarithm?
A logarithm answers the question:

To what power must a certain number (the base) be raised to produce another number?


Where:
- `b` = base
- `x` = result
- `y` = exponent

---

## ✅ Examples

| Expression        | Meaning     | Explanation                    |
|------------------|-------------|--------------------------------|
| `log₁₀(1000) = 3` | `10^3 = 1000` | Base 10 raised to 3 is 1000    |
| `log₂(8) = 3`     | `2^3 = 8`     | Base 2 raised to 3 is 8        |
| `log₁₀(1) = 0`    | `10^0 = 1`    | Any base raised to 0 is 1      |



