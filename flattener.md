# Problem - Array Flattener
![recursion](https://media.giphy.com/media/3GuP496Wrkos8/giphy.gif)

Imagine you have a deeply nested array, or multi-dimensional array, like this:

```rb
 array_of_ints = [1, 2, 3, [[4], 5], [[[6]]]]
 array_of_strings = ["hi", "this is", [[["string"], "that is very"], [[[["nested"]]]]]]
```
the contents of the array aren't important.

In Ruby and JS, we have built in methods and functions to `flatten` arrays into one dimension.  For example, in Ruby:

```rb
=> [1, 2, 3, [[4], 5], [[[6]]]]
[8] pry(main)> array_of_ints.flatten
=> [1, 2, 3, 4, 5, 6]
```
and in JS:

```js
> arr1
[ 0, 1, 2, [ 3, 4 ] ]
> arr1.flat()
[ 0, 1, 2, 3, 4 ]
```
If we look at the docs for either of these, we notice that they are _recursive_ by nature. Your goal is to recreate this functionality by writing a recursive function to accomplish this same thing. For example:

```rb
 array_of_ints = [1, 2, 3, [[4], 5], [[[6]]]]
=> [1, 2, 3, [[4], 5], [[[6]]]]
ruby_flattener(array_of_ints)
=> [1, 2, 3, 4, 5, 6]
```
or in JS:

```js
> arr1
  [ 0, 1, 2, [ 3, 4 ] ]
> flatten(arr1)
  [ 0, 1, 2, 3, 4 ]
```

# Instructions

1. Copy this markdown and paste in your own, privte gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom


## Rewrite the question in your own words:

Given a nested array, or a multi-dimensional array, write a function to 'flatten' the array in a single array.


## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?

That the elements in the input array have a length, input elements are numbers or strings.


## What are your initial thoughts about this problem? (high level design, 2-3 sentences)

Will need to use recursion to 'loop' through the array and extract each element adding it to single array.
Need to find a base case where there are no elements left in the array, i.e. array.length === 0.
Want a recursive case that removes elements of the array.


## How would you identify the elements of this problem?

- [ ] Searching of Data
- [X] Sorting of Data ??
- [ ] Pattern Recognition
- [ ] Build/Navigate a Grid
- [ ] Math
- [ ] Language API knowledge
- [ ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?
Use a single recursive function with a base case and a recursive case.

## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

pseduocode in repl

## Write out any implementation code OR link to repl

[REPL](https://replit.com/@AlexThompson207/Array-Flattener#index.js)

## What is the Big O complexity of your solution?
