# Read: 06 - JS Object Literals; The DOM

## Understanding the problem domain is the hardest part of programming

- Writing code is like putting together a jigsaw puzzle without clear instructions or vision
- Problem domains are difficult to understand and look completely different depending on your viewpoint
- Programming is easy if you understand the problem domain
- Understanding the problem domain(most critical piece of the equation), helps to write the code very easily 
- Very difficult to solve a problem before you know the question
- If domain seems too difficult, do two things:
  - Make the problem domain easier
    - Cutting out cases and narrowing your focus
  - Get better to understanding the problem domain
- It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.

## JS Chapter 3: “Object Literals” (pp.100-105)

- Functions allow you to group a set of related statements together that represent a single task. 
- What is an object?
  - Objects group together a set of variables and functions to create a model of something
  - Variables and function take on new names
    - Variables become properties
    - Functions become methods
- Creating an object: literal notation. Example below:
  - **this.** Keyword indicates that it is using the rooms and booked properties of this object

```
var hotel = {
	name: ‘Quay’,
	rooms: 40,
	booked: 25
	checkAvailability: function () {
	Return this.rooms - this.booked;
}
};
```

- Accessing an object using dot notation Example below:
  - You can also use bracket notation
    - Mostly used when:
      - Name of property or method contains special characters
      - Name of the property is a number
      - A variable is being used in place of the property name

```
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();
```

**OR**

```
var hotelName = hotel [‘name’];
var roomsFree = hotel [‘checkAvailability’]();
```

## JS Chapter 5: “Document Object Model” (pp.183-242)

- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes
  - Document nodes
    - Represents the entire page
  - Element nodes
  - Attribute nodes
  - Text nodes
- Select element nodes by their **id or class** attributes, by tag name or using CSS selector syntax. Examples below:
  - document.getElementById(‘one’)
  - querySelector()
- Whenever a DOM query can return more than one node, it will always return a NodeList. Examples below:
  - Two ways to select elements from a NodeList:
    - item() method
    - Array syntax

```
var elements = document.getElementByClass(‘hot’);
if (elements.length >= 1) {
	var firstItem = elements[0];
}
```

  - getElementByTagName(‘h1’)
  - getElementByTagName(‘li’)
  - getElementByClassName(‘hot’)
- From an element node, you can access and update its content using properties such as 
  - textContent
  - innerHTML
  - DOM manipulation techniques
- Looping through each node in the collection and applying the same statement to each. Example below:

```
var hotItems = document.querySElectorAll(‘li.hot’);
for (var i = 0; i < hotItems.length; i++) {
	hotItems[i].className = ‘cool’;
}
```

- An element node can contain multiple text nodes and child elements that are siblings of each other
  - Traversing the DOM
    - .parentNode
    - .previousSibling
    - .nextSibling
    - .firstChild
    - .lastChild
- Adding or removing HTML content. Two ways:
  - innerHTML
    - Gets the content of an element and return it as one long string
    - Higher risk but faster
  - DOM Manipulation Methods
    - Another technique to add new content to a page. Three steps: 
      - createElement()
      - createTextNode()
      - apprendChild()
- In older browsers, implementation of the DOM is inconsistent 
- Browsers offer tools for viewing the DOM tree

[Back to README](README.md)