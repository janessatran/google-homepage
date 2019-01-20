# google-homepage
From The Odin Project's [curriculum](http://www.theodinproject.com/courses/web-development-101/lessons/html-css



## Things I learned: 
1. Two ways to move a div around on the page

2. Stick a div onto the bottom or top of the page

3. Identify the background color of an existing webpage

4. Grab the URL for an image from an existing webpage

5. Center an element horizontally

6. Identify three ways you can include your CSS styles in a page
a. Inline CSS
Use the `style` attribute in HTML elements.
```html
<h1 style="color:red;">This is a red heading</h1>
```

b. Internal CSS
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

c. External CSS
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

7. Understand how to use classes and ids to target CSS at specific elements on the page

8. Build a very basic form (even if it doesn’t “go” anywhere)
