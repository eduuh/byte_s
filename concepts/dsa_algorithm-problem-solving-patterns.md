# Solving new problems

- Algorithm: A proces or set of steps to accomplish a certain task.

Almost everything that you do in programming involves some kind of Algorithm!
It's the foundation of being a succesful problem solving and developer.

## Problem Solving

1. Understand the problem
   - deliverate questions:
      1. Can I restate the problem in my own words? 
      2. What are the inputs that go into the problem
      3. What are the outpuss and should come from the solution.
      4. Can the outputs be determined from the inputes?
      5. How should I lable the impotant pieces of data that are part of the
         problem?.

2. Explore concrete examples
 
   - Coming up with example can help you understand the problem better.
   - Examples also provides sanity checks that you eventual solution works how
   it should.

3. Break it Down

   - Write some comments of steps you need to take.
   - This forces you to think about the code you'll write before you write it,
   and helps you catch any lingering conceptual issues or misunderstandings
   before you dive in and have to worry about details (e.g language syntax) as
   well.

4. Solve/simplify
5. Look back and Refactor

    - can you check the result?
    - can you derive the result differently?
    - can you undestand the solution at a glance
    - can you use the results or method for some other problem
    - Can you improve the performance of your solution?
    - Can you think of the other ways to refactor?
    - How have other people solved this problem?

### Example: Undestand the problem

Write a function which takes two numbers and return their sum

1. Can I restate the problem in my own words? 
    - "implement additions"

2. What are the inputs that go into the problem?
    - are working with two inputs?
    - are we working with many number?
    - are they super large numbers?

3. What are the outpuss and should come from the solution.
    - should it be a float string?

4. Can the outputs be determined from the inputes?
    - what happens if we do not have all number passed?

5. How should I lable the impotant pieces of data that are part of the
 problem?.


### Example: Explorer simple examples

1. Start with simple examples
2. Progress to more complex examples
3. Explore Examples with empty inputs
4. Explore examples with invalid inputs

### Write a function which takes in a string and returns counts of each
charactor in the string

- input: "Edwin"  output: 5 // charCount("Edwin") // {e: 1, d: 1, w: 1, n:1}

- input: "my phone number is 18877"
   - should we include numbers?
   - should we include spaces

- input: "My phone number is 18877"
    - should we ignore case?

- input: ""
   - how to handle empty string?

### Example Steps

```js
function charCount(str) {
    // make object to return at end
    // loop over string, for each charactor...
        //if the char is number/letter is a key in object , add one to count
        //if the char is number/letter not in object, add it and set value to 1
        //if character is something else (space, period, etc.) don't do anything
    // return an object 
}
```


### Solve/Simplify

- Solve the problem
- If you can't solve - Simplify. Ignore the part that giving you the hard time.
   - go for it.


- Find the core difficulty in what you're trying to do.
- Temporarily ignore that difficulty.
- Write a simplified solution.
- Then incorporate that difficulty back in.
