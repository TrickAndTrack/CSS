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
