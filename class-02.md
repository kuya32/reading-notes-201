<<<<<<< HEAD
# Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions

## HTML Chapter 2: “Text” (pp.40-61)

- HTML elements are used to describe the structure of the page 
Headings, subheadings, paragraphs
    - Headings come from ```<h1>```  to ```<h6>```	
- Additional HTML elements
    - ```<b>```
        - Bolds the texts
    - ```<i>```
        - Italizes the texts
    - ```<sup>```
        - Used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts
    - ```<sub>```
        - Used to contain characters that should be subscripted
    - ```<br />```
        - Adds a line break inside he middle of a paragraph
    - ```<hr />```
        - Creates a break between themes such as change of topics in a book or a new scene in a play
- **White space in HTML collapses!**
- They also provide semantic information
    - Where emphasis should be placed
    - The definition of any acronyms used
    - When given text is quotation
- Additional semantic markup tags
    - ```<strong>```
        - Indicates that its content has strong importance
        - Another way to “bold”
    - ```<em>```
        - Indicates emphasis that subtly changes the meaning of a sentence
        - Another way to “italicize” 
    - ```<blockquote>```
        - Used for longer quotes that take up an entire paragraph
    - ```<q>```
        - Used for shorter quotes that sit within a paragraph
    - ```<abbr>```
        - Used for abbreviations or an acronym
    - ```<cite>```
        - Used to indicate where the citation is from
    - ```<dfn>```
        - Used to indicate the defining instance of a new term
    - ```<address>```
        - Used to contain contact details for the author of the page
    - ```<ins>```
        - Used to show content that has been inserted into a document
    - ```<del>```
        - Show text that has been deleted from it
    - ```<s>```
        - Indicates something that is no longer accurate or relevant

## HTML Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

- CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look
- Rules are made up of selectors and declarations
- Different types of selectors allow you to target your rules at different elements
- Declarations are made of two parts:
    - The properties of the element that you want to change
    - The values of those properties
        - Ex. font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface
        - ```p { font-family: Arial;}```
- Additional selectors
    - Universal selector
        - Applies to all elements in the document
            - *{...}
    - Type selector
        - Matches element names
            - H1, h2, h3 {...}
    - Class selector
        - Matches an element whose class attribute has a value that matches the one specified after the period symbol
            - .note {...}
    - ID selector
        - Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol
            - #introduction {...}
    - Child selector
        - Matches an element that is a direct child of another
            - li > a {...}
    - Descendant selector
        - Matches an element that us a descendent of another specified element
            - p a {...}
- CSS rules usually appear in a separate document although they may appear within an HTML page
Advantages of using external style sheet
    * All web pages can share the same style sheet so no need to repeat the code
    * Once the user has downloaded the CSS stylesheet, the rest of the site will load faster
    * HTML code will be easier to read because less code overall on the sheet

## JS Chapter 2: “Basic JavaScript Instructions” (pp.53-84)

- A script is made up of a series of statements. Each statement is like a step in a recipe. 
- Scripts contains very precise instructions
    - Specify that a value must be remembered before creating a calculation using that value
    - Javascript is case sensitive
- Commits are used to explain what your code does
    - Multi-line comments
        - /* … */
    - Single line comments
        - //
- Variables are used to temporarily store pieces of information used in script
- The six rules for naming variables
    * The name must begin with a letter, dollar sign ($). It must not start with a number.
    * The name can contain letters, numbers, dollar sign ($), or an underscore (_). 
    * You cannot used keywords or reserved words
    * All variables are case sensitive
    * Use a name that describes the kind of information that the variable stores
    * Multiple word variable, use s capital letter for the first letter  of every word after the first word
- Array are special types of variable that store more than one piece of related information
    - Numbering items in an array
        - ```Colors = [ ‘white’, ‘black’, ‘custom’];```
            - Index number: ‘white’ = 0, ‘black’ = 1 and ‘custom’ = 2
    - Accessing items in an array
        - ```itemOne = colors[0];```
    - Number of items in an array
        - ```numColors = colors.length;```
- Javascript distinguishes between numbers (0-9), string (text), and Boolean value (true or false).
- Expressions evaluate into a single value
    - Two types  of expressions:
        - Expression that just assign a value to a variable
            - ```var color = ‘beige’;```
        - Expressions that use two or more values to return a single value
            - ```var area = 3 * 2;```
- Expressions rely on operators to calculate a value
- More operators
    - Increment (++)
        - Adds one to the current number
            - ```i = 10; i ++; --> i = 11```
    - Decrement (--)
        - Subtracts one from the current number
            - ```i = 10; i --; --> i = 9```
    - Modulus
        - Divides two values and returns the remainder
            - ```10 % 3,  Remainder = 1```

## JS Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)

- Conditional statements allow your code to make decisions about what to do next.
    - Comprised of two components:
        * An expression is evaluated, which returns a value
        * A conditional statement says what to do in a given situation
- Comparison operators (===, !==, ==, !=, <, >, <=, =>) are used to compare two operands.
    - Is equal to (==)
        - Compares two values to see if they are the same
    - Is not equal to (!=)
        - Compares two values to see if they are not the same
    - Strict equal to (===)
        - Compares two values to check that both the data type and value are the same
    - Strict not equal to (!==)
        - Compare two values to check that both the data type and value are not the same
    - Greater than (>)
        - Checks if the number on the left is greater than the number on the right
    - Less than (<)
        - Checks if the number on the let is less than the number on the right
    - Greater than or equal to (>=)
        - Checks if the number on the left is greater than or equal to the number on the right
    - Less than or equal to (<=)
        - Checks if the number on the left is less than or equal to number on the right
- Logical operators allow you to combine more than one set of comparison operators.
    - Logical and (&&)
        - Tests more than one condition
    - Logical or ( | | )
        - Tests at least one condition
    - Logical not (!)
        - Takes a single Boolean value and inverts it
- If … else statements allow you to run one set of code if a condition is true, and another if it is false.
    - If it resolves to true the first code block is executed. If the condition resolves to false the second code block is run instead

```
        If … else statement example:

	        If (score >= 50) {
	        	congratulated();
	        }
	        else {
	            encourage();
```
=======
[tag: paragraph]
>>>>>>> c85aa3ff5669eb3025f40485a0f2e8106f9fbb93
