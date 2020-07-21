# Read: 12 - Docs for the HTML <canvas> Element & Chart.js

[Article on the Chart.js API.](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)
- Utilizes the ```<canvas>``` element for charts.
- Chart.js is simple to use and very felxible. 

- [Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
  - Using ```<canvas> ``` element to create and manipulate content to focus on 2D/3D rendering. 

- [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
  - Utilizing the canvas grid or **coordinate space** which have x and y coordinates can help use create and draw shapes. 
  - ```<canvas>``` only supports two primitive shapes
    - Rectangles
    - Paths
  - Mathematical equations can be used to draw different shapes and images.

- [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
  - Two important properties we use:
    - fillStyle = Sets the style used when filling shapes
    - strokeStyle = Sets the style for shapes' outlines
  - There are numerous properties to explore for styling lines and shapes.
    - Shadowing, gradient, patterns and transparency are a few

- [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)
  - Canvas rendering contect provides two methods to render text:
    - fillText(text, x, y, maxWidth)
      - Fills a given textr at the given (x,y)position. Optionally with a maxiumum width to drtaw.
    - strokeText(text, x, y, maxWidth)
      - Strokes a given text at the ggiven (x,y) position. Optionally with a maximum width to draw. 
  - Some properties let us adjust the way the text gets diplated on canvas.
    - font = value
    - textAlign = value

[Back to README](README.md)