# Classes

Objectives:

1. Set up `HTML` and `CSS` files with css file link in head.
2. Test set up with a color change: body { background-color: blue; }
3. Reveal info about classes with the classes div.
4. Discuss rules of classes.
5. Discuss descendant selectors in `CSS`.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                01-classes.css
                01-classes.html
```

## Description <a id="description"></a>

Classes are one of the ways we have to target elements for styling in CSS. Using `class` allows you to apply thematic concepts to elements that can be easily modified. For example, if you want every `<button>` and every `<a>` tag to have the same text color, assigning a `class` allows you to specify a `value` for the property `color:` to that `class`. Let's explore this a little bit more by writing some HTML and assigning a `class` to several elements so we can see how classes can affect several elements using the same rules.

## Finished Code <a id="finished-code"></a>

HTML Code:

```text
<!DOCTYPE html>
<html>
  <head>
    <title>CSS Classes</title>
    <link rel="stylesheet" type="text/css" href="01-classes.css">
  </head>
  <body>
    <h1>HEY</h1>
    <div class="css-classes">
      <p>Make the background of this div light gray.</p>
    </div>
​
    <br>
​
    <div class="css-classes">
      <h1>To Do List</h1>
      <ul>
        <li>Run a marathon</li>
        <li>Get a coding job</li>
      </ul>
    </div>
​
    <div class="css-classes">
      <h3>Classes</h3>
      <p>A CSS Class is an identifier of an element which can be used multiple times on a page.</p>
      <p><b>Memory device:</b> Classes in school are periods. Remember to use a . whenever you want to reference a class.</p>
      <ul> 
        <li>Classes start with . in the selector <b>.anything-you-want-to-name-it</b></li> 
        <li>the same class name can be used more than once within the same file</li>
        <li>The class keyword refers to the class name that you set in the html page in the specific tag.</li>
        <li>In the CSS file, you can identify a class on the whole, or you can identify particluar parts to style (ex: p tags, h3, or li tags)</li>
      </ul>
    </div>    
  </body>
</html>
```

CSS Code:

```text
/*2*/
body {
    background-color: blue;
}
​
/*this styles everything within the css-classes class*/
.css-classes {
    background-color: lightgray;
}
​
/*this styles all the p tags within the css-classes class*/
.css-classes h1{
    font-size: 18px;
}
​
.css-classes p{
    font-size: 16px;
    color: green;
​
}
​
/*this styles all the li items within the css-classes class*/
.css-classes li{
    color: navy;
}
```

## Discussion <a id="discussion"></a>

Breaking down the code a little bit, let's first recognize that we've assigned a `class` of `"css-classes"` to all of the `<div>` tags above. Remember, `class` is an `attribute` that we can use to change the way HTML elements behave. Now we can delve into the `.css` file!

The first thing to identify in the `.css` file is that it's possible to reference generic HTML elements by their tag type.

We've done this by using the `selector` of `body`. This is followed by a `{` which indicates that we're **starting** our ruleset. We then move into the ruleset and choose a `property`. In the case of our `body` tag, we're choosing to change the `background-color:` and then we assign it the `value` of `blue`. If it isn't obvious, this states to the browser that all elements with a `<body>` tag will have a background that's blue. We state that the assignment is completed with a `;` at the end of the line. Finally, the ruleset is closed by a mated `}`. Just like in HTML, every opening `{` needs a closing `}` to let the browser know that we're done giving it instructions for the specific element/class.

Native HTML tags are one thing, but what about custom `.css` classes? Well, we identified `"css-classes"` a moment ago, and in the `.css` file we can see an entry with the same name. The only difference is that custom classes must be targeted using the `.` operator before the class name, as is reflected in the `.css` file above.

The last thing we need to discuss before moving on to the next lesson is descendant selectors. We know how to target a `class` using `.class`, but what if we want to target specific HTML elements in our `class`, but nowhere else? CSS has a neat trick where every element type that is a child can be easily pointed at by appending the element type to the end of our `class`. This is reflected with the syntax `.css-classes h1` in our code above.

## Challenge <a id="challenge"></a>

Try adding a `property` to one of your selectors above. Explore some of the properties that we haven't discussed yet...there are quite a few of them!

## More Reading <a id="more-reading"></a>

A great CSS example, if needed, can be found [here](https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_selectors).

