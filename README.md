# google-homepage
From The Odin Project's [curriculum](http://www.theodinproject.com/courses/web-development-101/lessons/html-css).
You can check out my completed work for this assignment [here](https://janessatran.github.io/google-homepage/)!

## Things I learned: 
### Two ways to move a div around on the page
**Relative positioning**: changes the position of the HTML element relative to where it normally appears. 

**Absollute positioning**: An element with position: absolute is positioned at the specified coordinates relative to your screen top-left corner.

**Fixed positioning**: Fixed positioning allows you to fix the position of an element to a particular spot on the page, regardless of scrolling. Specified coordinates will be relative to the browser window.
<br>

### Stick a div onto the bottom or top of the page
Fixed bottom: 
```css
div {
    position: fixed;
    bottom: 0;
    width: 100%;
}
```
Fixed top: 
```css
div {
    position: fixed;
    bottom: 0;
    width: 100%;
}
```
<br>
### Identify the background color of an existing webpage
Use inspect tool -> look for `background-color` attribute in css.
<br>

### Grab the URL for an image from an existing webpage
Use inspect tool -> hover over image and click inspect. 
<br>

### Center an element horizontally
To center an image, set left and right margin to `auto` and make it into a `block` element:
```html
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 40%;
}
```
<br>

### Identify three ways you can include your CSS styles in a page
#### Inline CSS
Use the `style` attribute in HTML elements.
```html
<h1 style="color:red;">This is a red heading</h1>
```

#### Internal CSS
Use the `<style>` element in `<head>` section. 
```html
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: white;}
h1   {color: red;}
p    {font-size: 12px ;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

#### External CSS
Use an external CSS file. To use an external stylesheet, link it in the `<head>` section of the HTML. 

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
This is what the style.css file would look like:
```css
body {
  background-color: white;
}
h1 {
  color: red;
}
p {
  font-size: 12px;
}
```
<br>

### Understand how to use classes and ids to target CSS at specific elements on the page
In the CSS, a class selector is a name preceded by a full stop (“.”) and an ID selector is a name preceded by a hash character (“#”). The difference between an ID and a class is that an ID can be used to identify one element, whereas a class can be used to identify more than one.

**IDs** are unique: 
- Each element can have only one ID
- Each page can have only one element with that ID

**Classes** are not unique: 
- You can use the same class on multiple elements.
- You can use multiple classes on the same element.

The following style rule will be applied to the element with id "para1":
```html
para1 {
  text-align: center;
  color: red;
}
```

The following style rule will be applied to all elements with class "center":
```html
.center {
  text-align: center;
  color: red;
}
```

You can also specify that only specific HTML elements should be affected by a class. The following will be applied to only p elements with class "center": 
```html
p.center {
  text-align: center;
  color: red;
}
```
<br>

### Build a very basic form (even if it doesn’t “go” anywhere)
To build a search form, we use an `input` element.

```html
  <input type="text" placeholder="Search..">
```
Then you can style the element in css by specifying rules in `input` like:
```css
    /* Style search box */
    input {
        background-color: transparent;
        margin-left: auto;
        margin-right: auto;
        font-size: 12px;
        display: block;
        width: 50%;
        padding-top:10px;
        padding-bottom: 10px;
        margin-top:10px;
        padding-left: 10px;
        -webkit-tap-highlight-color: transparent;
    }
```
