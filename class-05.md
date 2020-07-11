# Read: 05 - HTML Images; CSS Color & Text

## HTML Chapter 5: “Images” (pp.94-125)

- The ```<img>``` element is used to add images to a web page.
- You must always specify an **src** attribute to indicate the source of an image and an **alt** attribute to describe the content of an image.
  - Also can adjust the image size with height and width
    - Better to manipulate the width only for non squished images
- Three rules for creating images
  * Save images in the right format
  * Save images at the right size
  * Measure images in pixels
- You should save images at the size you will be using them on the web page and in the appropriate format
- Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.
  - Many different colors = JPEG
  - Few colors or large area of same color = GIF and PNG

## HTML Chapter 11: “Color” (pp.246-263)

- Color not only brings your site to life, but also helps convey the mood and evokes reactions
- There are three ways to specify color in CSS:
  - RGB values
  - Hex codes
  - Color names
- Color picker can help pick the color you want
- It is important to ensure that there is enough contrast between any text and the backgroundcolor
  - Otherwise people will not be able to read it
  - Levels of contrast depends on situation of user and creators intention of content
- CSS3 has introduced an extra value for RGB colors to indicate opacity. Known as RGBA
  - Opacity allows you to specify the condition of lacking transparency or translucence of an element
- CSS3 also allows you to specify colors as HSL values, with an optional opacity value. Known as HSLA.
  - Opacity (rgba)
    - Specify the opacity of an element and any of its child elements
  - New specifications
    - Hue
      - The colloquial idea of color
    - Saturation
      - The amount of gray in a color
    - Lightness values
      - The amount of white (lightness) or black (darkness) in a color
    - HSL & HSLA
      - Hsl - an alternative way to specify color
      - Hsla - specify color properties like before but adds a value which represents transparency

## HTML Chapter 12: “Text” (pp.264-299)

- There are properties to control the choice of:
  - Font (view examples on page 269-270)
    - Serif
    - San-serif
    - Monospace
    - Cursive 
    - Fantasy
    - Size
    - Weight
      - Adds emphasis and affect the amount of white space and contrast
    - Style
    - Spacing
- Type of scales
  - Pixels
  - Percentages 
  - Ems
    - Allow you to change the size of text relative to the size of the text in the parent element
- There is a limited choice of fonts that you can assume most people will have installed.
- Manipulation of fonts
  - Font-weight
    - Allows to create bold text
      - Normal 
      - Bold
  - Font-style
    - Allows to create italic text
      - Normal
      - Italic 
      - Oblique
  - Text-transform
    - Used to change the case of text 
      - Uppercase
      - Lowercase 
      - Capitalize
  - Text-decoration
    - Allows you to specify one of the following:
      - None
      - Underline
      - Overline
      - Line-through
      - Blink
- If you want to use a wider range of typefaces there are several options, but  you need to have the right license to use them.
- You can control the space between lines of text, individual letters and words.
  - Kerning
    - Use letter-spacing or word-spacing in CSS
- Text can also be aligned to the left, right, center and justified. It can also be indented.
  - Text-align
    - Allows you to control alignment of text
  - Vertical-align
    - More commonly used with inline elements such as ```<img>```, ```<em>```, or ```<strong>``` elements. 
- More manipulation on texts with CSS
  - Text-indent
    - Allows you to indent the first line of text within an element
  - Text-shadow 
    - Used to create a drop shadow, which is a dark version of the word just behind it and slightly offset. 
- You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link. 
  - Link
    - Allows to set styles for links that have not been visited
  - Visited
    - Allows to set styles for links that have been clicked on
  - Hover
    - Applied when the user hovers over an element with a pointing device such as a mouse
  - Active
    - Applied when an element is being activated by a user
  - Focus 
    - Applied when an element has focus

[Back to README](README.md)