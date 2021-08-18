# React Docs - lists and keys

What does .map() return?
**returns a new array containing the resulting values of running the operation on each element.**

If I want to loop through an array and display each value in JSX, how do I do that in React?
**use the map() function to take an array**

Each list item needs a unique _**Key**___.

What is the purpose of a key?
**Keys help React identify which items have changed, are added, or are removed.**

# The Spread Operator

What is the spread operator?
***The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.***

List 4 things that the spread operator can do.
- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Adding an item to a list

## Give an example of using the spread operator to combine two arrays.
const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

## Give an example of using the spread operator to add a new item to an array.
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌"

## Give an example of using the spread operator to combine two objects into one ]

[1,3,5].min() // undefined
Math.min([1,3,5]) // NaN
Math.min().apply(null, [1,3,5]) // 1
Math.max().apply(null, [1,3,5]) // 5

[My Readme file page](README.MD)