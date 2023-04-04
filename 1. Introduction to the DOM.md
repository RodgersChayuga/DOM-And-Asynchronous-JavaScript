# 1. Introduction to the DOM:
#### 1. What is the DOM?
Is a Document Object Model, which is a programming interface for HTML and XML documents.

#### 2. How does the DOM relate to HTML and CSS?
It represents the web page or XML document as a tree-like structure where each node in the tree represents an object in the document.

#### 3. How does JavaScript interact with the DOM?
Javascript can interact and manipulate the DOM using a set of built-in methods and properties. These methods and properties allow Javascript to access, create, modify, and delete HTML elements, attributes, and text nodes on a web page. 

#### 4. Examples of common DOM manipulations (e.g. changing text, adding/removing elements)
**4.1. Changing Text:** You can change the text of an element using the `textContext` property.
For example, to change tht text of a paragraph element with the ID `"my-para"`, you could use the following code:

```Javascript
document.getElementById("my-para").textContent = "New text"
```

**4.2. Adding Elements:** You can add new elements to the DOM using the `createElement` method, and then add them to the the page using the `appendChild` method. For example, to add a new paragraph element to a div element with the ID `"my-div"`, you could use the following code:

```Javascript
const newPara = document.createElement("p"); //creting a paragraph element
const textNode = document.createTextNode("New paragraph"); // add text or paragraph

newPara.appendChild(textNode): //add the text in the paragraph element.
document.getelementById("my-div").appendChild(newPara); //update the `my-div` ID with the new paragaraph.
```

**4.3. Removing Elements:** You can remove elements from the DOM using the `removeChild` method. For example, to remove a paragraph element with the ID `"my-para"`, you could ude the following code: 

```Javascript
const para = document.getElementById("my-para"); // Get the intended element by it's ID name
para.parentNode.removeChild(para); //Get to the parent of the element to be removed, and specify the child to be removed.
```

**4.4. Changing Attribute:** You can change the attributes of an element using the `serAttribute` method. For example, to change the href attribute of a link element with the ID `"my-link"`, you could use the following code:

```Javascript
document.getElementById("my-link").setAttribute("href", "https://www.example.com");
```


**4.5. Changing CSS:** You can change the style properties of an element using the `style` property. For example, to change the background color of a div element with the ID `"my-div"`, you could use the following code:

```Javascript
document.getElementById("my-div").style.backgroundColor = "red";
````

**4.6. Changing Classes:** You can add or remove classes from an element using the classList property. For example, to add a class "active" to a div element with the ID `"my-div"`, you could use the following code:

```Javascript
document.getElementById("my-div").classList.add("active");
````

Similarly, to remove a class `"inactive"` from the same div element, you could use the following code:

```Javascript
document.getElementById("my-div").classList.remove("inactive");
````

**4.7. Event Handling:** You can add event listeners to elements using the `addEventListener` method. For example, to add a click event listener to a button element with the ID `"my-button"`, you could use the following code:

```Javascript
document.getElementById("my-button").addEventListener("click", function() {alert("Button clicked")}); // the addEventListener takes in two arguments, the event in this case it is a click, and a function that throws an alert message.
````

**4.8. Creating and Setting Attributes:** You can create new attributes on an element using the `setAttribute` method. For example, to add a data attribute `data-user-id` to a div element with the ID `"my-div"`, you could use the following code:

```Javascript
document.getElementById("my-div").setAttribute("data-user-id", 12345); // setAttribute takes in two arguments the key of the attribute in this case is "data-user-id" and it's value, in this case "12345"
````

Similarly, you can retrieve the value of an attribute using the `getAttribute` method. For example, to get the value of the `"data-user-id"` attribute of the same div element, you could use the following code:

```Javascript
const userId = document.getelementById("my-div").getAttribute("data-user-id");
````

These are just a few more examples of the many ways you can manipulate the DOM using JavaScript. The DOM provides a powerful and flexible API for building dynamic web applications.
