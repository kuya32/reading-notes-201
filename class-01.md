# Read: 01 - Introductory HTML and JavaScript

## HTML Chapter 1: “Structure” (pp.12-39)

- HTML pages are text documents
- HTML uses tags to give information they surround special meanings
    - ***body***, ***head***, and ***title*** tags
- Another way to say tags is “elements”
- Tags come in pairs. Opening tag denotes the start of a piece of content; closing tag denotes the end

```
    -<p> - opening tag for a paragraph
    - </p> - closing tag for a paragraph
```

- Opening tags can carry attributes, which tell us more about the content of that element

```
    - <p id=”banana”> - this shows a tag with a identity attribute of banana
    - <p class=”apple”> - this shows a tag with a class attribute of apple
```

- Attributes require a name and value

## HTML Chapter 8: “Extra Markup” (p.176-199)

- DOCTYPE tell browser which version of HTML you are using

```
- <!DOCTYPE html> tells the browser we are using HTML5
```

- You can add comments to your code between the <!-- and → markers
    - Use comments to explain parts of code in HTML
- The *id* and *class* attributes allow you to identify particular elements

```
- <p id=”banana”> - this shows a tag with a identity attribute of banana
    - <p class=”apple”> - this shows a tag with a class attribute of apple
```

    - These attributes can be used to easily manipulate through CSS
- The ***div*** and ***span*** elements allow you to group block-level and inline elements together
    - Other block elements
        - ***h1***, ***p***, ***ul*** and ***li***
    - Other inline elements
        - ***a***, ***b***, ***em***, and ***img***
- ***iframes*** cut windows into your web pages through which other pages can be displayed
    - When using ***iframe*** also identify the width, height and source (src) of the image
- The ***meta*** tag allows you to supply all kinds of information about your web pages
    - Description of web page for search engines to use.

## HTML Chapter 17: “HTML5 Layout” (pp.428-451)

- The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure
- The new elements provide clearer code
    - Traditional HTML used numerous ***div*** to structure its web page
    - HTML5 corrects the overuse of ***div*** and writes with cleaner and organized code
- New tags/elements
    - ***header***
        - Located at the top of page
        - Contains the site name and the main navigation
    - ***footer***
        - Located at the bottom of page
        - Contains copyright information
    - ***nav***
        - Used to contain the major navigational blocks on the site such as the primary site navigation
    - ***article***
        - Acts as a container for any section of a page that could stand alone and potentially be syndicated
    - ***aside***
    - ***section***
        - Groups related content together, and typically each section would have its own heading
        - Leave containing elements for the entire page to ***div***
    - ***hgroup***
        - To group together a set of one or more ***h1*** through ***h6*** elements so that they are treated as one single heading
    - ***figure***
    - ***figcaption***
    - ***div*** 
        - Important way to group together related elements

## HTML Chapter 18: “Process & Design” (pp.452-475)

- It's important to understand a couple things when producing your HTML web page
    - Who is your target audience?
        - Your web page can't please everyone so try to focus on one group
    - Why would they come to your site?
        - Most will visit for a specific reason
        - Look for key goals and motivations
    - What information do they want to find?
        - Think of reasons why people would join the site 
        - Then prioritize levels of information
    - When are they likely to return?
        - Depending on information, the web page might need to be updated more frequently than others
- Site maps allow you to plan the structure of a site
    - Helps decide what information should be included and go on each page
- Wireframes allow you to organize the information that will need to go on each page
    - This is the diagram of how you want your webpage to look like
    - Helps imagine information in specific areas of the webpage
- Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell the
    - Content - So much different aspects of information is included in a webpage
        - Prioritizing
            - Making parts of the page **distinct** from surrounding content, designers draw attention to (or away from) those items
        - Organizing
            - Grouping together related content into **blocks or chunks** make the page look simpler
- You can differentiate between pieces of information using:
    - Size
        - Larger elements grabs the users attention
    - Color
        - Foreground and background color can draw attention to key messages
    - Style
        - Different style of lettering (bold and italic) can separate content to stand out
- You can use grouping and similarities to help simplify the information you present
    - Grouping related pieces of information together can make a design easier to comprehend
        - Proximity
            - Items placed close together
        - Closure
            - A recognizable pattern or form
        - Continuance
            - Lined or curved content perceives as related
        - White space
            - Closer and larger gaps help with grouping
        - Color
            - Background color placed behind content emphasizes their connection
        - Borders
            - Visually see they are grouped together
- You can help make the user process easier by setting up a good navigation design on web page

## JS Chapter 1: “The ABC of Programming” (pp.11-52)

- How javascript makes web pages more interactive
    - Access content
    - Modify content
    - Program rules
    - React to events
- Writing a script
    - Define the goal
    - Design the script
    - Code each step
- A script is a series of instructions that the computer can follow in order to achieve goals
- Computer approach task in different ways, so instruction is needed
- Expressions - evaluates into (results in) a single value. Broadly speaking there are two types of expressions
    - var color = ‘beige’;
    - var area = 3 * 2
_________________________________________________________

- Computers create models of the worlds using data
    - A video game of chess
- The models use objects to represent physical things
    - Objects can have
        - Properties
            - Tells us about the object
        - Methods
            - Perform tasks using the properties of that object
        - Event
            - Triggered when a user interacts with the computer
- Programmers can write code to say:
    - “When this event occurs, write this code.”
- Web browsers use HTML markup to create a model of a web page.
    - Each element creates its own node (which is a kind of object)
- To make web pages interactive, you write code that uses the brower’s model of the web page.
_________________________________________________________

- Keep Javascript in their own file
    - Javascript files are text files that are labeled with “.js” extension
    - HTML is labeled with “.html” and CSS is labeled with “.css” extension
- The HTML ***script*** element is used in HTML pages to tell the browser to load the Javascript file
```
    - **Ex. <script src=”js/add-content.js”></script>**
    - Example of CSS in HTML pages:
        - <link rel=”stylesheet” href=”css/co1.css” />
            - Placed in the <head>
```

- ### VERY IMPORTANT: Placement of ***script*** for .js is before the ***closing body*** tag
    - The script is not blocking other things from downloading
    - The DOM has already loaded by the time the script is executed
- View source code of browser Javascript will not have changed the HTML because script works with model of web page the browser has created

[Back to README](README.md)