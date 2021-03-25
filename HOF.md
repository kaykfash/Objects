#Explain High Order Function with example:

A Higher Order functions are functions that receives a function as an argument or returns the function as output.
Higher order functions operate on other functions, either by taking them as arguments or by returning them. 
Higher-order functions allows you to write simpler and more elegant code.

#Example of High Order Function:
Array.map()
forEach()
Array.filter()
Array.reduce()
Array.sort()


#Explain the map and reduce method with Example:

#Map() method

The map() method is used for creating a new array from an existing one, applying a function to each one of the elements of the first array. Generally map() method is used to iterate over an array and calling function on every element of array.
Syntax:
Let  new_array = arr.map(function callback(element, index, array) {
    // Return value for new_array
}[, thisArg])


Example:
In this example , each element(boysAge) of an array is doubled

const boysAge = [15, 17, 19, 16];
const doubled = boysAge.map(age => age * 2);
console.log(doubled); 
// [ 30, 34, 38, 32 ]


#Reduce() Method
The reduce() method reduces an array of values down to just one value. To get the output value, it runs a reducer function on each element of the array.


Syntax:
arr.reduce(callback[, initialValue])



Example:
const girlsAge = [1, 2, 3, 4,6];
const sum = girlsAge.reduce(function (result, item) {
  return result + item
});

console.log(sum)
// 10
