# A basic A-Frame scene

The HTML page [index.html](./index.html) contains a basic 3D scene created using the [A-frame](https://aframe.io/) library. The whole scene is a single HTML file; HTML files are files containing webpages. 


Documentation for A-Frame is available from https://aframe.io/docs/master/introduction/


## Editing using a sandbox

There are many sandbox environments on the web preconfigured to edit html+javascript code. To open any github repo in [codesandbox.io](https://codesandbox.io) change the url from `github.com/[...]` to `githubbox.com/[...]`. Note that any changes you do will be stored on [codesandbox.io](https://codesandbox.io) and will not be contributed back to this repository.

Once you open this repository in [codesandbox.io](https://codesandbox.io), your sandbox will look like this. 
<p align="center"><img src="https://user-images.githubusercontent.com/7040974/214770151-1ac1abf4-a76e-4991-a0e5-b353be9eedc7.png"
alt="Sandbox view" width="400em" /></p>

From left to right you see: 
- a file and configuration pane 
- a file (html) editor 
- a live preview of your webpage

You can close the left pane and pop out the live preview into a separate tab if you want more screen real-estate for editing
<p align="center"><img src="https://user-images.githubusercontent.com/7040974/214770573-b0d5bbf3-5a81-4b28-b3a3-96066fbf5160.png" width="300em"
/> </p>

To make and save your changes to the sandbox you have to form it. 
<p align="center"><img src="https://user-images.githubusercontent.com/7040974/214770251-13e2dcb3-f6e8-41ab-bfe5-514794470649.png"
alt="fork button in the sandbox environment"
width="200em" /></p>

Next, let us look at the html source code and identify the main parts. 

## Basic HTML

You can find a basic introduction to html mark-up in [a html crash course](https://www.w3schools.com/html/html_intro.asp). HTML is a *document markup language* not a programming language. HTML does not contain any logic. The programming language used for the web is Javascript. It is tightly integrated with HTML and allows you to execute commands in your browser that alter the html contents of the displayed website. 

### Tags

Content in html are organized in a heirarchically into tags. Tags to delimit meaningful parts of a website. For example, this is a valid piece of HTML:

```html
<body>
<section> 
    <!-- This is a comment, it is ignored when rendering the webpage. 
    The tag immediately in front of this is an opening of a section. 
    Each tag has to be closed by the "closing" tag that starts with the / character
    -->
    <h1> This is the header of level 1 </h1>
    <p> This is a paragraph that is contained inside the p tags </p>
</section>
</body>
```

### A-Frame and external libraries

The library A-Frame, used for creating immersive graphical websites is pulled in through the `<script>` tag in the header of this html file.

```html
<head>
    <!-- ... -->
<script src="https://aframe.io/releases/1.4.0/aframe.min.js"></script> 
    <!-- ... -->
</head>
```
The library is not stored on your computer, it is downloaded from the internet by your browser.

