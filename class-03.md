# Read: 03 - HTML Lists, CSS Boxes, JS Control Flow

## HTML Chapter 3: “Lists” (pp.62-73)

- There are three types of HTML lists: ordered, unordered, and definition
    * Ordered lists (```<ol>```) use numbers 
        - Each item in the list is placed between an opening ```<li>``` and closing ```</li>``` tag
    * Unordered (```<ul>```) lists use bullets
        - ```<li>``` is also used for unordered lists
    * Definition lists (```<dl>```) are used to define terminology
        - Consists of a series of terms and their definitions
        - ```<dt>```
            - Contain the term being defined
        - ```<dd>```
            - Used to contain the definition
- List can be nested inside one another
    - Just add an addition order/unordered tags within list

## HTML Chapter 13: “Boxes” (pp.300-329)

- CSS treats each HTML element as if it has its own box.
- You can use CSS to control the dimensions of a box.
    - Overflow
        - Tells the browser what to do if the content contained within a box is larger than the box itself. Two values: hidden and scroll
            * Hidden: Simply hides any extra content that does not fit in the box.
            * Scroll: Adds a scrollbar to the box so that users can scroll to see the missing content.

```
    p.one {
	    overflow: hidden;}
    p.two {
	    overflow: scroll;}
```

- You can also control the borders, margin and padding for each box with CSS.
    - Borders
        - Separates the edge of one box from another
        - More info for borders on p. 309-312
    - Margin
        - Sits outside the edge of the border
        - More info for margin on p. 314
    - Padding
        - The space between the border of a box and any content contained within it.
        - Adding padding can increase the readability of its content. 
        - More info for padding on p. 313
- It is possible to hide elements using the display and visibility properties.
    - Visibility property allows you to hide boxes from users but it leaves a space where the element would have been
- Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
    - Example on p. 317
- Legibility can be improved by controlling the width of boxes containing text and the leading.
- CSS3 has introduced the ability to create image borders and rounded borders. 
    - border-image 
        - Applies an image to the border of any box
        - Example on p. 319
    - box -shadow
        - Allows you to add a drop shadow around the box
        - Example on p. 320
    - border-radius 
        - Creates rounded corners on any box
        - Can also mess with the degree of the box corners
        - Example on p. 321-322

## JS Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)

- If … else statements allow you to run one set of code if a condition is true, and another if it is false.
    - If it resolves to true the first code block is executed. If the condition resolves to false the second code block is run instead
- Switch statement allow you to compare a value against possible outcomes
- Data styles can be coerced from one type to another.
    - Ex. a string ‘1’ could be converted to a number 1 in the follow expression:‘1’ > 0
        - Above expression would evaluate to true
- All values evaluate to either truthy or falsy
    - Falsy values are treated as if they are false
        - Ex. ```var highScore;```
            - A variable with no value assigned to it.
        - More examples found p. 167
    - Truthy values are treated as if they are true
        - Examples found on p. 167
- There are three types of loop: for, while and do...while. Each repeats a set of statements. 
    - For loop
        - Used when you need to run code a specific number of times
    - While loop
        - Used when you don't know how many times the code should be ran
    - Do...while loop
        - Same is while loop, but with one difference. It will always run the statement at least once. Even if the condition evaluates to false.
    - Example of a for loop:


    for (var i = 0; i < 10; i++) {
        document.write(i);
    }


    - For loop breakdown:
        - Initialization (var i = 0;)
            - Variable is commonly called i, and it acts as the counter
        - Condition (i < 10;)
            - The loop should continue to run until the counter reaches a specified number
        - Update (i++)
            - Every time the loop has run the statement in the curly braces, it adds one to the counter

[Back to README](README.md)