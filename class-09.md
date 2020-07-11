# Read: 09 - Forms and Events

## HTML Chapter 7: “Forms” (p.144-175)

- World’s best known form is the search box
  - Several types of form control
    - Adding text
    - Making choices
    - Submitting Forms
- Whenever you want to collect information from visitors you will need a form, which lives inside a ```<form>``` element. Examples for all these tag elements on p. 151-168
  - ```<form>``` - form control
    - Should always carry an action attribute whose value is the URL for the page on the server that will receive the information in the form when it is submitted 
  - ```<input>```
    - Used to create several different form controls
      - type=’password’ 
        - Attribute that creates a text box that acts just like a single-line text input 
      - type=’radio’
        - Allows the users to pick just one of a number options
      - type=’checkbox’
        - Allows users to select one or more options in answer to a question
      - type=’file’
        - Creates a box that looks like a text input followed by a browse button
      - type=’submit’
        - Used to send a form to the server
      - type=’image’
        - Use an image for a submit button
      - type=’date’
        - Asking user for a date
  - ```<button>```
    - Allows users more control over how their buttons appear and to allow other element to appear inside the button
  - ```<textarea>```
    - Used to create a multi-line text input
  - ```<select>``` 
    - Drop down list that allows users to select one option from a drop down list.
  - ```<option>```
    - Used to specify the options that the user can select from
  - ```<label>``` 
    - Used in two ways:
      - Wrap around both the test description and the for input
      - Be kept separate from the form control
  - ```<fieldset>```
    - Group related form controls together 
  - ```<legend>```
    - Contains the opening caption which helps identify the purpose of that group of form controls
- Information from a form is sent in name/value pairs.
- Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
- HTML5 introduces new form elements which make it easier for visitors to fill in forms.
  - ```<input>```
    - type=’email’
      - Used to ask users email
    - type=’url’
      - When asked user for a web page address
    - type=’search’
      - Creates a single line textbox for search queries

## HTML Chapter 14: “Lists, Tables & Forms” (pp.330-357)

- In addition to the CSS properties covered in other chapters which work with the contents of all elements, there are several others that are specifically used to control the appearance of lists, tables, and forms.
- List markers can be given different appearances using the list-style-type and list-style image properties
  - List-style-type
    - Allows you to control the shape of style of a bullet point
      - Unordered lists
        - Ex. None, disc, circles, squares
      - Ordered lists
        - Ex. decimals, decimals-leading-zero, lower- and upper alpha, lower- and upper-roman
  - List-style image
    - Specifies an image to act as a bullet point 
  - List-style-position
    - Indicates whether the marker should appear on the inside or the outside of the box containing the main point
      - Outside
        - Marker sits to the left of the block of text
      - Inside
        - Marker sits inside the box of text
  - List-style
    - Shorthand of writing CSS rule
- Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
  - Example of table properties are listed on p. 337-338
- Forms are easier to use if the form controls are vertically aligned using CSS. 
- Forms benefit from  styles that make them feel more interactive. 
  - More examples and information of CSS styling with forms on p. 341-346

## JS Chapter 6: “Events” (pp.243-292)

- Events are the browser’s way of indicating when something has happen
  - Such as when page has finished loading or a button has been clicked
- Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
- When an event occurs on an element, it can trigger a Javascript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
- You can use event delegation to monitor for events that happen on all of the children of an element.
- The most commonly used event are W3C DOM events
  - Although there are others in the HTML5 specifications as well as browser-specific events

[Back to README](README.md)