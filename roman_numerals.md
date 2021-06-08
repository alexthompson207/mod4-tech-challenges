# Problem - Roman Numerals
![Roman Numerals](https://media.giphy.com/media/xT5LMNd1ieywmnI3Qc/giphy.gif)

[What are Roman Numerals?](https://www.mathsisfun.com/roman-numerals.html)

Write a function that converts an integer into a string such that the number is represented in Roman Numerals in the most efficient way.

For example, the number `4` could be written as `IIII` but it's more efficient to use `IV`since that's a shorter string.

Assume no number is greater than 4,000.

Here are the Roman Numeral equivalents you'll need to know:
- M=1000
- CM=900 
- D=500 
- CD=400
- C=100 
- XC=90 
- L=50 
- XL=40
- X=10 
- IX=9 
- V=5 
- IV=4 
- I=1

## JS Starter Code
```js
function toRoman(num) {
  // your code goes here
}

console.log(toRoman(128));  // should return "CXXVIII"
console.log(toRoman(2000)); // should return "MM"
console.log(toRoman(2017)); // should return "MMXVII"
console.log(toRoman(1999)); // should return "MCMXCIX"
```

## Ruby Starter Code
```rb
def to_roman(num)
  # your code goes here
end

puts to_roman(128)   # should return "CXXVIII"
puts to_roman(2000)  # should return "MM"
puts to_roman(2017)  # should return "MMXVII"
puts to_roman(1999)  # should return "MCMXCIX"
```

# Instructions

1. Copy this markdown and paste in your own, privte gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom

Do not publish your code on a public repl.it or repo or other public means.

## Rewrite the question in your own words:

Given a number input, write a function that transforms number into roman numeral string.


## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?

Assume that input is a number, postive, and whole. Numbers range from 0 - 4000.

## What are your initial thoughts about this problem? (high level design, 2-3 sentences)

There could be some type of pattern to identify. 
Seems like there could be endless conditionals if no pattern exists.
Maybe can break the number up based on if it's greater or less than 50, 100, -- roman numeral characters.


## How would you identify the elements of this problem?

- [ ] Searching of Data
- [ ] Sorting of Data
- [ X ] Pattern Recognition
- [ ] Build/Navigate a Grid
- [ ] Math
- [ ] Language API knowledge
- [ X ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?

At the moment I cannot see structure without many conditionals, this not great for performance.
Need to identify pattern, not sure if I'll need to iterate or not.


## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

- create an object with keys of roman numerial and values of their respective numeric values
- create an empty results array to hold roman numerial strings
- Iterate over object keys
- divide input num by roman numerial equivalent and look for positive remainder 
- If remainder is positive, subtract number from number input and add corresponding key to result array
- continue loop until finsihed 
- return string of results

## Write out any implementation code OR link to repl

[REPL](https://replit.com/@AlexThompson207/Roman-Numerials#index.js)

## What is the Big O complexity of your solution?

I think it's O(n) or O (log n), but not sure...
