# Read: 07 - HTML Tables; JS Constructor Functions

## Domain Modeling

- Domain modeling
  - The process of creating a conceptual model in code for a specific problem
  - Contains
    - Various entities 
    - Attributes and behaviors
    - Constraints
- Object-oriented programming
  - An entity that stores data in properties and encapsulates behavior in methods
  - The ```new``` keyword instantiates (creates) an object
  - The constructor function initializes properties inside that object using the ```this``` variable.
  - The object is stored in a variable for later use. 
- Constructor function’s **prototype.** Example shown below: 
  - Think of a prototype as an object’s stunt double.
  - When a prototype is shared between two or more objects those objects execute the same code when the method is called. 
    - Shared code means a running program consumes less memory

```
EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);
```

- Summary
  - Model its attributes with a constructor function that dines and initializes properties.
- Model its behavior with small methods that focus on doing one job well
- Create instances using the ```new``` keywords followed by a call to a constructor function
- Store the newly created object in a variable so you can access its properties and methods from **outside.**
- Use the ```this``` variable within methods so you can access the object’s properties and methods from **inside.**

## HTML Chapter 6: “Tables” (pp.126-145)

- ```<table>``` element is used to add tables to a web page.
- A table is drawn out row by row. 
  - Each row is created with the ```<tr>``` element.
- Inside each row there are a number of cells represented by the ```<td>``` element 
  - Or ```<th>``` if it is a header
- You can make cells of a table span more than one row or column using the **rowspan** and **colspan** attribute.
  - **rowspan** attribute can be used on a ```<th>``` or ```<td>``` element to indicate how many rows a cell should span down the table. 
  - **colspan** attribute can be used on a ```<th>``` or ```<td>``` element and indicates how many columns that cell should run across.
  - For long tables you can split the table into a ```<thead>```, ```<tbody>```, and ```<tfoot>```. 
  - ```<thead>```
    - Houses the heading of the table 
  - ```<tbody>```
    - Houses the body
  - ```<tfoot>```
    - Houses the footer

## JS Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

- Creating an object: Constructor Notation
  - New keyword and object constructor create a blank object
    - Then add properties and methods to the object. Example below:

```
var hotel = new Object();
hotel.name = ‘Quay’;
hotel.rooms = 40;

hotel.checkAvailability = function() {
	return this.rooms - this.book;
};
```

  - Use dot notation or square brackets
    - hotel.name = ‘Park’;
    - hotel[‘name’] = ‘Park’;
- Creating many objects: Constructor Notation
  - Object constructors can use a function as a **template** for creating objects. Example below:

```
function Hotel (name, rooms, booked) {
	this.name = name;
	this.rooms = rooms;
	this.booked = booked;
	
	this.checkAvailability = function() {
		return this.rooms - this.booked;
};
}
```

  - ```this``` keyword indicates that the property or method belongs to the objects that **this** function creates. 
- Create **instances** of the object using the constructor function
  - **new** keyword followed by a call to the function creates a new object.
  - Properties of each object are given as arguments to the function. Example below:

```
var quayHotel = new Hotel(‘Quay’, 40, 25);
var parkHotel = new Hotel(‘Park’, 120, 77);
```

  - Adding and removing properties. Example below:

```
hotel.gym = true;
hotel.pool = false;
delete hotel.booked; 
```

- Object Model
  - Group of objects, each of which represent related things from the real world
- Web browsers implement objects that represent both the browser window and the document loaded into the browser window. **Browser Object Model**
  - Creates a model of the browser tab or window. 
  - Top of the tree is **Window object** which represents current browser window or tab
    - **Child objects** represent other browser features
- **Document Object Model**
  - Creates a model of the current web page
  - Topmost of tree is the **document object**
    - **Child objects** represent tiger items on the page
- **Global Javascript Objects**
  - Javascript also has several built-in objects that make up the model such as:
    - String
      - For working with string values
    - Number 
      - For working with numeric values
    - Math 
      - For working with boolean values
    - Date
      - To represent and handle dates
    - Math
      - For working with numbers and calculations
    - Regex
      - For matching patterns within strings of text
  - **Examples and method descriptions of all three groups of built-in objects on p.124-139**
- Their properties and methods offer functionality that help you write scripts.
- Arrays and objects can be used to create complex data sets. 
  - Arrays in an objects and vice versa

[Back to README](README.md)