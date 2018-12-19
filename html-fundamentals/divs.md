# Divs

In this module we will do the following:

1. Discuss div tag.
2. A few notes on divs. Reviewing ul.
3. Create div-one and discuss lorem ipsum.
4. Create additional divs with styling.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
                07-divs.html <---You should be here.
```

## Description <a id="description"></a>

The `<div>` tag defines a division in an HTML document. The `<div>` tag is used to group block-elements to format them with CSS or JavaScript. By default, browsers always place a line break before and after the `<div>` element. However, this can be changed with CSS.

## Sample Code <a id="sample-code"></a>

This is an opportune moment to discuss lorem ipsum: Lorem Ipsum is filler text frequently used to demonstrate how an element will be presented when it is populated with content. Though derived from an ancient Latin text, there are many flavors of Lorem Ipsum that exist now, including [Cupcake Ipsum](http://www.cupcakeipsum.com/). Since this lesson is about the `<div>` tag and is **not** a typing exercise, feel free to copy/paste the Lorem Ipsum which we've placed inside of the `<p>` tags below. Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>divs</title>
</head>
<body>
    <h1>Div tags</h1>
    <ul>
        <li>Help organize layout</li>
        <li>Help with DOM manipulation</li>
        <li>Often seen with classes(more on these later)</li>
    </ul>
​
    <h1>Examples</h1>
    <div class="div-one">
        <h2>Div One</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
​
    <div class="div-two" style="border:1px solid black">
        <h2>Div Two</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
​
    <div class="div-three" style="background-color: gray">
        <h2>Div Three</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
</body>
</html>
```

## Discussion <a id="discussion"></a>

Let's break this block of code down a little bit: You're probably starting to get used to reading code by now, and can recognize that we created a list at the top of our file and then created a series of divs that each contain an `<h2>` and a `<p>` tag. Our second and third divs have some minor inline styling and are rendered differently by the browser as a result.

## Uses <a id="uses"></a>

The `div` tag is everywhere you look. You'll use it in all your projects. This section addresses the fundamentals of this tag, but be prepared to see divs in every project you work on.

## Challenge <a id="challenge"></a>

Try creating new divs and altering the inline styling of the ones you've just made.

