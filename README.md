# Introduction to the DOM:
#### 1. What is the DOM?
Is a Document Object Model, which is a programming interface for HTML and XML documents.
#### 2. How does the DOM relate to HTML and CSS?
It represents the web page or XML document as a tree-like structure where each node in the tree represents an object in the document.
#### 3. How does JavaScript interact with the DOM?
Javascript can interact and manipulate the DOM using a set of built-in methods and properties. These methods and properties allow Javascript to access, create, modify, and delete HTML elements, attributes, and text nodes on a web page. 
#### 4. Examples of common DOM manipulations (e.g. changing text, adding/removing elements)
**a. Changing Text:** You can change the text of an element using the `textContext` property.
For example, to change tht text of a paragraph element with the ID `"my-para"`, you could use the following code:

```Javascript
document.getElementById("my-para").textContent = "New text"
```

**b. Adding Elements:** You can add new elements to the DOM using the `createElement` method, and then add them to the the page using the `appendChild` method. For example, to add a new paragraph element to a div element with the ID `"my-div"`, you could use the following code:

```Javascript
const newPara = document.createElement("p"); //creting a paragraph element
const textNode = document.createTextNode("New paragraph"); // add text or paragraph

newPara.appendChild(textNode): //add the text in the paragraph element.
document.getelementById("my-div").appendChild(newPara); //update the `my-div` ID with the new paragaraph.
```
