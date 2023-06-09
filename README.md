# CSS
Cascading Style Sheets is a style sheet language used for describing the presentation of a document written in a markup language such as HTML or XML. CSS is a cornerstone technology of the World Wide Web, alongside HTML and JavaScript
 

 ### Targeting & Background
   Use two types of colors. use a hex color which is a color represention written in hexadecimal, or you can use RGB or RGBA and RGB is kind.

body is an element.
if we use color so it will apply to text only

```
body{

   background: #00ff00;
  //background: #cc0000;
  // background: #0000aa;
  // background: #000000;
  // background: #aa0000;
  
  color: #0af 
  or
  // color: #00aaff

  

}
```

// Targeting

```
h3{
     color: green;
  }

body p{

   color: white;
}

 ```

### Element specificity


```
<style>
  p {
    color: blue; /* Specificity: 1 type selector */
  }
  
  .container p {
    color: red; /* Specificity: 1 class selector + 1 type selector */
  }
  
  #special-paragraph {
    color: green; /* Specificity: 1 ID selector */
  }
</style>

<div class="container">
  <p>This paragraph will be red.</p>
  <p id="special-paragraph">This paragraph will be green.</p>
</div>


```

### ID targeting, margin, and border

- `FONT` we use the font-family property to specify the font of a text.


##### CSS section

```
<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:ital@1&display=swap');

body{
   font-family:'Roboto Mono', ital;
   font-weight: 400;


}

body h1{
   font-weight:300;
}

#special-paragraph{
   border: 1px solid black;
}

</style>
```
- `IDTargeting` ID targeting in CSS refers to the use of the ID selector to select and apply styles to a specific HTML element on a web page.
```
<style>

#special-paragraph{
   border: 1px solid black;
}

</style>
```


##### HTML section
```

<div class="container">
  <p>This paragraph will be red.</p>
  <p id="special-paragraph">This paragraph will be green.</p>
</div>

```
- border The CSS border properties allow you to specify the style, width, and color of an element's border.

### Padding, margin, and float

- `Margins` are used to create space around elements, outside of any defined borders.
- `Padding` is used to create space around an element's content, inside of any defined borders.

##### HTML & CSS section
```
<style>

#special-paragraph{
   border: 1px solid black;
}
.container{
   color: blue;
   margin: 10px;
   margin-top: 20px;
   padding: 20px 10px 5px 20px;
   

}
</style>

<div class="container">
  <p>This paragraph will be red.</p>
  <p id="special-paragraph">This paragraph will be green.</p>
</div>
```

- `float` property is used to specify how an element should float within its parent container. When an element is floated, it is moved to one side of its container and allows other content to flow around it.

The float property accepts the following values:

none (default): The element does not float, and content flows around it according to the normal document flow.

left: The element is floated to the left side of its container. Content to the right of the floated element wraps around it.

right: The element is floated to the right side of its container. Content to the left of the floated element wraps around it.
```
.float-example {
  float: left;
  width: 200px;
  height: 200px;
  margin: 10px;
}

.clearfix::after {
  content: "";
  display: table;
  clear: both;
}

```
![image](https://github.com/TrickAndTrack/CSS/assets/73180409/7f0c6037-6b6b-44fb-acd3-b1a6ae6b0f68)

### Max- width and Background-images

This Example is background image for the entire page:
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url('TrickAndTrack.jpg');
}
</style>
</head>
<body>

<h1>Background Image</h1>

<p>By default, the background image will repeat itself if it is smaller than the element where it is specified, in this case the body element.</p>

</body>
</html>

```
This Example is background image for Specify Content in the HTML body

```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  background-image: url('TrickAndTrack.jpg');
  max-width:30%
  height: 100px;
 }
</style>
</head>
<body>

<h2>Background Image</h2>

<p>You can specify background images<br>
for any visible HTML element.<br>
In this example, the background image<br>
is specified for a div element.<br>
By default, the background-image<br>
will repeat itself in the direction(s)<br>
where it is smaller than the element<br>
where it is specified. (Try resizing the<br>
browser window to see how the<br>
background image behaves.</p>

</body>
</html>
```

### Text Decoration 
text-indent: The text-indent property specifies the indentation of the first line in a text-block.
test-shadow: 


```
p{
  word-Spacing:2px;
  latter-Spacing: 2px
  text-indent: 20px;
  text-shadow: 2px 5px 5px #000; 
  // shadow will go upside
  text-shadow: 2px -5px 5px #000; 
}
```
### Pseudo-states

The `hover` selector is used to select elements when you mouse over them.
> The `hover` selector can be used on all elements, not only on links.
> Use the :link selector to style links to unvisited pages, the :visited selector to style links to visited pages, and the :active selector to style the active link.

```
<!DOCTYPE html>
<html>
<head>
<style>
/* unvisited link */
a:link {
  color: red;
}

/* visited link */
a:visited {
  color: red;
}

/* mouse over link */
a:hover {
  color: green;
}

/* aftar selected link */
a:active {
  color: blue;
} 
</style>
</head>
<body>

<p> Mouse over and click the link: 
<a href="https://github.com/TrickAndTrack"> TrickAndTrack </a>
</p>

</body>
</html>

```

### Focus & Border Redius

The :focus selector is used to select the element that has focus.

The Border Radius is used to corner convert into a curve.

```
<!DOCTYPE html>
<html>
<head>
<style>
input:focus {
  background-color: yellow;
  color: #0000;
  outline: none;
  border: 1px solid #000;
  border-redius:3px;
  border: 1px solid transperant;
}
</style>
</head>
<body>

<h1>Demo of the :focus selector</h1>

<p>Click inside the text fields to see a yellow background:</p>

<form>
  First name: <input type="text" name="firstname"><br>
  Last name: <input type="text" name="lastname">
</form>

</body>
</html>
```
### Z-index

