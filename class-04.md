# Read: 04 - HTML Links, CSS Layout, JS Functions

## HTML Chapter 4: Ch.4 “Links” (pp.74-93)

- Links are created using the ```<a>``` element.
- The ```<a>``` element uses the href attribute to indicate the page you are linking to.
  - Ex. ```<a href=”http://www.imdb.com”> IMDB</a>```
- If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.
- You can create links to open email programs with an email address in the “to” field.
  - Ex. ```<a href=”mailto: m.acode@outlook.com”>Email Marchael</a>```
- You can use the id attribute to target elements within a page that can be linked to. Example below:

```
<h1 id=”top”> Film-Making Terms</h1>
<a href=”#arc_shot”>Arc Shot</a><br />
<a href=”#interlude”> Interlude</a><br />

<h2 id=”arc_shot”> Arc Shot</h2>
	Informations about Arc Shot
<h2 id=”interlude”>Interlude</h2>
	Information about Interlude
```

## HTML Chapter 15: “Layouts” (pp. 358-404)

- ```<div>``` elements are often used as containing elements to group together sections of a page.
  - Block level elements
    - ```<h1>```, ```<p>```, ```<ul>```, and ```<li>```
  - Inline elements
    - ```<img>```, ```<b>```, and ```<i>```
- Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning 
  - Relative
    - Moves an element in relation to where it would have been in normal flow.
  - Absolute
    - The box is taken out of normal flow and no longer affects the position of other elements on the page.
  - Fixed
    - Type of absolute positioning 
    - Positions the element in relation to the browser window
    - When a user scrolls down the page, it stays in the exact same place.
- The float property moves content to the left or right of the page and can be used to create multi-column layouts. 
  - Floated items require a defined width so they don't take up full length of page
  - Using float to place elements side-by-side
    - Height of boxes affects where elements sit
  - Clearing floats (clear: left;)
    - Allows you to say that no element should touch the left or right hand side of a box
  - Creating multi-column layouts with floating
    - Using ```<div>``` to section content, then width, float and margin in CSS to space out content between each other
- Z-index allows you to control which box appears on top.
  - Value of z-index is a number 
  - Higher/larger number will appear over the top of smaller numbers
- Pages can be fixed width or liquid (stretchy) layouts. 
  - Fixed width layouts design
    - Do not change size as the user increases or decreases the size of their browser window.
    - Advantages:
      - Accurate pixel values when controlling size and position of elements
      - Far greater control of items appearance and position
      - Control the lengths of lines of text regardless of size
      - Size of image stays the same	
    - Disadvantages
      - Large gaps at ends of pages
      - Higher resolution users can't see text and is hard to read
      - Increase in font size, text might not fit
      - Only works better with devices with similar resolution
      - Takes more vertical space
  - Liquid layouts design
    - Stretch and contract as the user increases or decreases the size of their browser window
    - Advantages:
      - Page expands so no spaces around the page
      - Small window, page contracts to fit
      - Tolerant of users setting, larger font sizes
    - Disadvantages
      - If width is not controlled, expected results won't show
      - Wide window causes stretched text
      - Narrow window causes squished text
      - Large image plus small box means overflow
- Designer keeps pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels
  - To demonstrate its relevance without scrolling
- Grids help create professional and flexible designs.
  - 960 pixel grid
  - Continuity across different pages and designs
  - Helps user find information on page
  - Easier to add new content
  - Helps collaborate the site 
- CSS frameworks provide rules for common tasks. 
  - 960 Grid System
  - Available at www.960.gs
  - Advantages
    - Save you from repeating code
    - Tested across different browser versions
  - Disadvantages
    - Require use class names in your HTML code that only control presentation of page
  - Contain more code than you need for your particular web page
- You can include multiple CSS files of one page. 

## JS Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)

- Function allows you to group a set of related statements together that represent a single task. Example of a function is shown below. 

```
<!--Creates function-->
Function sayHello() {
	Document.write (“Hello!”);
}
<!--Calls function-->
sayHello();
```

- Functions can take parameters (information required to do their job) and may return a value. Example shown below.

```
Function getArea(width, height) {
	Return width * height;
}
```

- Getting a single value out of a function shown below

```
function calculateArea(width, height) {
	var area = width * height;
	return area;
}
var wallOne = calculateArea(3, 5);
var wallTwo = calculateArea(8, 5);
```

- Getting multiple values out of a function shown below

```
function getSize(width, height, depth) {
	var area = width * height;
	var volume = width * height * depth;
	var sizes = [area, volume];
	Return sizes;
}
var areaOne = getSize(3, 2, 3) [0];
var volumeOne = getSize(3, 2, 3) [1];
```

- Variable scope
  - Local variable (local scope)
    - When a variable is created inside a function using the var keyword, it can only be used in the function
    - Can not be used outside the function
  - Global variable (global scope)
    - If you create a variable outside a function, then it can be used anywhere within the script.

## Article: “6 Reasons for Pair Programming”

- Pair programming involves two roles:
  * The Driver
    - The programmer who is typing and the only one whose hands are on the keyboard
  * The Navigator
    - Uses their words to guide the Driver but does not provide any direct input to the computer
    - Thinks of big picture and look up solutions
- Four fundamental skills that help anyone learn a new language
  * Listening 
    - Hearing and interpreting the vocabulary
      - Developers explain out loud what the code should do
  * Speaking
    - Using the correct words to communicate an idea
      - Listen to others’ guidance
  * Reading
    - Understanding what written language intends to convey
      - Read code that others have written
  * Writing
    - Producing from scratch a meaningful
      - Write code themselves
- Greater efficiency
  - Produces higher-quality code with less bugs
  - Run into a problem, both are looking for a solution
  - Enhances technical skills, team communication and enjoyable coding in the workspace
- Engaged collaboration
  - Harder to procrastinate when someone else is relying on you to complete work
  - Help additional help is right in front of you
- Learning from fellow students
  - Get a different perspective and learn a new technique
  - More experience coders help less experienced coder and both benefit through interaction
- Social skills
  - Helps improve communication skills which are long term career impacts for hiring process
- Job interview readiness
  - The ability to work with and learn from others and stellar communication skills are as important to a company than specific technical skill
  - ***TALK ABOUT PAIR PROGRAMMING IN INTERVIEW!!!***
- Work environment readiness
  - Code Fellows graduates have an advantage in the tech world!
