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

* **slice() -** returns a new array with a selected portion of the original array

```Javascript
// Declare an array with some elements
let myArray = ["apple", "banana", "cherry", "orange", "grape"];

// Extract a portion of the array using slice()
let slicedArray = myArray.slice(1, 4);

// Display the extracted portion and the original array
console.log(slicedArray); // Output: ["banana", "cherry", "orange"]
console.log(myArray); // Output: ["apple", "banana", "cherry", "orange", "grape"]
```

* **splice() -** adds or removes elements from an array at a specified index position

```Javascript
// Declare an array with some elements
let myArray = ["apple", "banana", "cherry", "orange", "grape"];

// Remove an element from the array using splice()
let removedElement = myArray.splice(2, 1);

// Add elements to the array using splice()
myArray.splice(1, 0, "pear", "kiwi");

// Display the modified array and the removed element
console.log(myArray); // Output: ["apple", "pear", "kiwi", "banana", "orange", "grape"]
console.log(removedElement); // Output: ["cherry"]
```

* **concat() -** joins two or more arrays and returns a new array.

```Javascript
// Declare two arrays
let array1 = ["apple", "banana", "cherry"];
let array2 = ["orange", "grape"];

// Concatenate the two arrays using concat()
let concatenatedArray = array1.concat(array2);

// Display the concatenated array and the original arrays
console.log(concatenatedArray); // Output: ["apple", "banana", "cherry", "orange", "grape"]
console.log(array1); // Output: ["apple", "banana", "cherry"]
console.log(array2); // Output: ["orange", "grape"]
```

* **sort() -** sorts the elements of an array in place, either alphabetically or numerically

```Javascript
// Declare an unsorted array
let unsortedArray = ["orange", "apple", "grape", "banana", "cherry"];

// Sort the array using sort()
let sortedArray = unsortedArray.sort();

// Display the sorted and unsorted arrays
console.log(sortedArray); // Output: ["apple", "banana", "cherry", "grape", "orange"]
console.log(unsortedArray); // Output: ["apple", "banana", "cherry", "grape", "orange"]
```

* **filter() -** creates a new array with all elements that pass a certain test.

```Javascript
// Declare an array of numbers
let numbers = [2, 4, 7, 9, 10, 12, 15];

// Use filter() to get even numbers
let evenNumbers = numbers.filter(function(number) {
  return number % 2 === 0;
});

// Use filter() to get numbers greater than 10
let greaterThanTen = numbers.filter(function(number) {
  return number > 10;
});

// Display the filtered arrays
console.log(evenNumbers); // Output: [2, 4, 10, 12]
console.log(greaterThanTen); // Output: [12, 15]
```

* **map() -** creates a new array with the results of calling a function for every array element.

```Javascript
// Declare an array of numbers
let numbers = [2, 4, 6, 8, 10];

// Use map() to create a new array with each number multiplied by 2
let doubledNumbers = numbers.map(function(number) {
  return number * 2;
});

// Use map() to create a new array with each number squared
let squaredNumbers = numbers.map(function(number) {
  return number ** 2;
});

// Display the new arrays
console.log(doubledNumbers); // Output: [4, 8, 12, 16, 20]
console.log(squaredNumbers); // Output: [4, 16, 36, 64, 100]
```

* **reduce() -** applies a function to each element of an array and reduces the array to a single value.

```Javascript
// Declare an array of numbers
let numbers = [2, 4, 6, 8, 10];

// Use reduce() to calculate the sum of all the numbers in the array
let sum = numbers.reduce(function(accumulator, currentValue) {
  return accumulator + currentValue;
});

// Display the sum
console.log(sum); // Output: 30
```
