# 3. Overview of array methods:

### 1. What are array methods?

**An Array:** Is a data structure that contains a collection of elements, of the same data type, which
can be acceessed by their index positions.

**Array Methods:** are built-in functions in programming languages, such as Javascript, 
that allow for manipulation and management of arrays.

>Array methods provide an easy and efficient way to perform operations on arrays, 
such as adding or removing elements, sorting, filtering, and reducing.


### 2. Examples of common array methods in javascript.
* **push() -** Adds one or more elements to the end of an array and returns the new length of the array.

```Javascript
// Declare an empty array
let myArray = [];

// Add elements to the array using push()
myArray.push("apple");
myArray.push("banana");
myArray.push("cherry");

// Display the array
console.log(myArray); // Output: ["apple", "banana", "cherry"]
```

* **pop() -** Removes the last element from an array and returns that element.

> We will use the Array above.

```Javascript
// Declare an array with some elements
let myArray = ["apple", "banana", "cherry"];

// Remove the last element from the array using pop()
let removedElement = myArray.pop();

// Display the modified array and the removed element
console.log(myArray); // Output: ["apple", "banana"]
console.log(removedElement); // Output: "cherry"
```

* **shift() -** Removes the first element from an array and returns the element.

```Javascript
// Declare an array with some elements
let myArray = ["apple", "banana", "cherry"];

// Remove the first element from the array using shift()
let removedElement = myArray.shift();

// Display the modified array and the removed element
console.log(myArray); // Output: ["banana", "cherry"]
console.log(removedElement); // Output: "apple"
```

* **unshift() -** adds one or more elements to the beginning of an array and returns the new length of the array

```Javascript
// Declare an array with some elements
let myArray = ["apple", "banana", "cherry"];

// Add elements to the beginning of the array using unshift()
myArray.unshift("orange", "grape");

// Display the modified array
console.log(myArray); // Output: ["orange", "grape", "apple", "banana", "cherry"]
```
