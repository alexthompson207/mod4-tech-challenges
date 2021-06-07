# Problem - Next Palindrome
Any number that reads the same way forwards as it does backwards is a palindrome. For instance, `12321` would be considered a palindrome, whereas `123` would not be. 

Write a function that takes in an integer and returns the next palindrome. For instance:

```js
findNextPalindrome(100)
// should return 101
```

and 

```js
findNextPalindrome(101)
// should return 111
```

# Instructions

1. Copy this markdown and paste in your own, private gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom


## Rewrite the question in your own words:

Given a number input find the next number that is a palindrome, forwards and backwards.


## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?

That no numbers are negative, the input is a whole number, and not letters or symbols are used. What are the limits of the input?

## What are your initial thoughts about this problem? (high level design, 2-3 sentences)

Need to write logic to check if a number is a palindrome or not.
Need to use some type of loop and break out of it when next palindrome is found.


## How would you identify the elements of this problem?

- [X] Searching of Data
- [ ] Sorting of Data
- [ ] Pattern Recognition
- [ ] Build/Navigate a Grid
- [ ] Math
- [ ] Language API knowledge
- [ ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?
Need to create a for loop to iterate over potential next number that is palindrome, set start of for loop to number input.
Check each number to see if it's a palindrome or not, maybe use `reverse()` method if it is allowed. Otherwise use a reverse for loop.

## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

// Input is a positive whole number
// Use for loop to loop through n + 1, n + 2,..... of next input to see if it is a palindrome or not.
// maybe start loop at 0 to check if input is a palindrome first
// reverse found palindrome number using reverse method
// break out of loop and return number (i) that is a palindrome.

## Write out any implementation code OR link to repl

```
const findNextPalindrome = (input) => {

  for (let i = 1; i >= 1; i++) {
    let isPalindrome = input + i;
    
    if (isPalindrome.toString().split('').reverse().join('') === isPalindrome.toString()) {
      return isPalindrome;
      
    }
  }
}
```

[REPL](https://replit.com/@AlexThompson207/Next-Palindrome#index.js)

## What is the Big O complexity of your solution?

Either O(n) I think
