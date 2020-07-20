# Read: 11 - Assorted Topics

## HTML Chapter 16: “Images” (pp.406-427)

- You can specify the dimensions of images using CSS.
  - This is very helpful when you use the same sized images on several pages of your site.
- Images can be aligned both horizontally and vertically using CSS.
  - New classes are created with names such as ***align-left*** or ***align-right*** to align the images to the left or right of the page. 
  - Setting ```margin: 0px auto``` centers images
- You can use a background image behind the box created by any element on a page.
  - background-image 
    - Allows you to place an image behind any HTML element
  - background-attchment
    - Specifies whether a background image should stay in one position, fixed, or move as the user scrolls up and down the page, scroll. 
- Background images can appear just once or be repeated across the background of the box.
  - background-repeat + four values (repeat, repeat-x, repeat-y, no repeat)
    - Background image is repeated both horizontally and vertically
- You can create image rollover effects by moving the background position of an image.
- To reduce the number of images your browser has to load, you can create image sprites.
- If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible. 

## HTML Chapter 19: “Practical Information” (476-492)

- Search engine optimization helps visitors find your sites when using search engines.
- How to determine keywords and steps to brainstorming on p. 481-482
- Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.
- To put your site on the web, you will need to obtain a domain name and web hosting.
  - Domain name - your web address
  - Web Hosting - upload to a web server which is constantly connected to the internet
- FTP (File Transfer Protocol) programs allow you to transfer files from your local computer to your web server.
  - Popular FTP applications
    - FileZilla
    - FireFTP
    - CuteFTP
- Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).

## This MDN article on audio and video elements

- ```<video>``` and ```<audio>``` elements allow us to embed video and audio into web pages. Old way:

```
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```

    - Attribute **controls** enables the default set of playback controls. If you don't specify this, you get no playback controls.
- ```HTMLMediaElement``` API makes a wealth of functionality available for creating simple video and audio players.
- Use JavaScript, CSS and HTML to structure an interactive video/audio player on a web page.

## HTML Chapter 9: pages 201-206 only. Flash is no longer supported by many browsers but is an important part of history.

- Since the 1990s, flash has been a very popular tool for creating animations, and later for playing audio and video on websites.
- Web technologies change quickly, **like hella fast!**

[Back to README](README.md)