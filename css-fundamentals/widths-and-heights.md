# Widths & Heights

Objectives:

* To study width and height in CSS.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                06-widths-heights.css
                06-widths-heights.html
```

## Sample Code <a id="sample-code"></a>

Let's go ahead and set up our HTML and CSS files. Make sure your HTML file looks like below:

```text
<!DOCTYPE html>
<html>
  <head>
    <title>Width and Height</title>
    <link rel="stylesheet" type="text/css" href="06-widths-heights.css">
  </head>
  <body>
    <div class="wrapper"></div>
  </body>
</html>
```

Here is the sample CSS Code:

```text
.wrapper{
    margin: 5px;
}

h1{
    text-align: center;
}
```

## Discussion <a id="discussion"></a>

Let's start talking about width and height. This is how we can shape the size of our HTML elements. There are a couple of different ways we can size things, we can use percentages, or explicit sizes like pixels. There is also `auto` which is the default way to size things, this means that the browser calculates the size.

Let's add some notes to our HTML right underneath our wrapper div:

```text
<h1>Width and Height</h1>
<p>The width and height properties are used to set the width and height of an element.</p>
<p>The default setting for width and height is auto, which means the browser decides the width and height.</p>
<p>Other settings for width and height are:</p>
<ul>
  <li>specified length values such as px & em</li>
  <li>percent of the containing div (ex: 50%, 100%)</li>
</ul>
```

## More Examples <a id="more-examples"></a>

Let's look at a few examples. Add the following underneath your notes in your `html`:

```text
<div class="example1">
    <p>This element has a width of 50% and height of 200px.</p>
</div>
```

So, let's style this div to give it a width of 50% and a height of 200px. See if you can do this yourself in CSS, then check below. Also, give the div a background color of something so you can really see the size.

Check and see if your CSS matches below!

```text
.example1{
    height: 150px;
    width: 50%;
    background-color: cornflowerblue;
}
```

Let's do another example, starting with saving the picture from [here](https://www.oregonhikers.org/field_guide/File:Mt._Hood,_Timothy_Lake.jpg), save the image as lake.jpg for ease of reference in your HTML.

Add the following to your HTML, right before your closing wrapper div tag.

```text
<div class="example2">
    <p>You can also manipulate width and height with images. This image was originally approx 400px x 200px, now it's 400px x 400px.</p>
    <img src="../4-assets/lake.jpg">
</div>
```

Let's style this image using width and height in our css. Again, see if you can figure out how to do it, and then check the CSS below.

```text
.example2 img{
    width: 400px;
    height: 400px;
}
```

Feel free to play with the values here, to see how these values affect the size of different elements.

Your files should look like the finished files below.

## Finished Code <a id="finished-code"></a>

HTML:

```text
<html>
  <head>
    <title>Width and Height</title>
    <link rel="stylesheet" type="text/css" href="06-widths-heights.css">
  </head>
  <body>
    <div class="wrapper">
      <h1>Width and Height</h1>
      <p>The width and height properties are used to set the width and height of an element.</p>
      <p>The default setting for width and height is auto, which means the browser decides the width and height.</p>
      <p>Other settings for width and height are:</p>
      <ul>
        <li>specified length values such as px & em</li>
        <li>percent of the containing div (ex: 50%, 100%)</li>
      </ul>
​
      <div class="example1">
        <p>This element has a width of 50% and height of 200px.</p>
      </div>
​
      <div class="example2">
        <p>You can also manipulate width and height with images. This image was originally approx 400px x 200px, now it's 400px x 400px.</p>
        <img src="../4-assets/lake.png">
      </div>
    </div>
  </body>
</html>
```

CSS:

```text
.wrapper{
    margin: 5px;
}
​
h1{
    text-align: center;
}
​
.example1{
    height: 150px;
    width: 50%;
    background-color:cornflowerblue;
}
​
.example2 img{
    width: 400px;
    height: 400px;
}
```

Next, we'll talk about borders.

