# Positions



Objectives for this module include the following:

1. Discuss the different position properties.
2. Discuss z-index and stacking order on an html page.
3. Experiment with position.

## File Location <a id="file-location"></a>

Your files should be located as follows:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                08-positions.css
                08-positions.html
```

We'll start with creating a basis in our HTML file. Open `08-positions.html`, and start off with the following code. We're creating a few divs to style and show the different positions.

```text
<!DOCTYPE html>
<html>
  <head>
    <title>Position</title>
    <link rel="stylesheet" type="text/css" href="08-positions.css">
  </head>
  <body>
    <div class="wrapper">
      <div class="nav"></div>
      <div class="positioning"></div>
      <div class="lotsoftext"></div>
    </div>
  </body>
</html>
```

Now, let's set up the CSS file. Head over to your `08-positions.css` file, and start with the following CSS.

```text
.wrapper{
    margin: 5px;
}
```

## Fixed Positions <a id="fixed-positions"></a>

Now, let's start to talk about position. Let's start with `fixed` position. Add this following `<p>` tag to your `nav` div.

```text
<p>this div has a fixed position</p>
```

Now, let's work on styling it. Head over to your `0.08_position.css` file, and start with the following CSS. If you notice our html `<p>` tag says "fixed position, so let's start with the position property in our CSS.

```text
.nav{
    position: fixed;
}
```

If you had to guess, what do you think "fixed" position means? It means that an element with `position: fixed`; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The `top`, `right`, `bottom`, and `left` properties are used to position the element.

So, right now, we don't have any of the properties on it, so we'll need to assign those. Make your `nav` css look like this:

```text
.nav{
    position: fixed;
    top: 0;
    right: 0;
    width: 250px;
    background-color: lightgray;
    border: 3px solid navy;
}
```

Notice how we've used `top: 0` and `right: 0` in addition to `position: fixed`. The 0 next to `top` and `right` means that we are positioning this fixed element at the 0 position top and right, which means that it should be all the way right and all the way to the top, 0 amount away from the top and right. The other properties here are just styling our `.nav` element to have a width of 250 pixels, with a background color of light gray, and a navy border.

To really see this in action we'll need some more text on the screen to be able to see it staying in the same place while scrolling. Add the following text to our `lotsoftext` div. After adding this, you should be able to see how the navbar stays fixed.

```text
<div class="lotsoftext">
    <h2>Here is some text, so you can scroll and see the div with a fixed position example.</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
    quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
    consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
    cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
</div>
```

Try changing the "top" and "right" properties and notice how the position changes, for example change top to `150px` and see what happens.

Let's take some notes on these positions. In our `0.08_position.html` file, let's add a list to the "positioning" div. Let's start with the following in the `positioning` div.

```text
<div class="positioning">
    <h1>Position</h1>
    <p>The position property specifies the type of positioning method used for an element. The four position values are:</p>
    <ul></ul>
</div>
```

In our `<ul>` let's add our first list item talking about `fixed` positioning. Add the following inside of your `<ul>` tag.

```text
<li><b>fixed:</b> this will pin something to a spot, and it will stay there as you scroll. (ex: nav bar) Fixed position takes elements out of the normal document flow.</li>
```

Let's add the rest of our styling, make sure to add these to your css file.

```text
.positioning{
    width: 75%;
    background-color: lightgray;
}
​
.positioning h1{
    text-align: center;
}
​
.lotsoftext{
    text-align: left;
    background-color: lightblue;
    width: 75%;
}
```

Change your `nav` styling back to `top: 0` and `right: 0` if you haven't already and let's move on.

## Static Positioning <a id="static-positioning"></a>

Static position will be how things are positioned by default. Let's add a new `<li>` to our `<ul>` with some notes on static position.

```text
<li><b>static:</b> this is the default setting, it is not affected by top, bottom, left, and right properties. It is always positioned according to the normal flow of the page.</li>
```

Static position will be the how your items are positioned unless you specify another positioning.

## Relative Positioning <a id="relative-positioning"></a>

Add the following list item to your unordered list, then we'll talk through it.

```text
<li><b>relative:</b> does not take the element out of normal document flow. Still appears within its space/div/container, but allows it to be offset a bit from the top, bottom, right, left. Top, right, bottom, and left properties will move it away from its normal position. Other content will not be adjusted to fit into any gap left by the element.</li>
```

Relative positioning is similar to static, but you can move things with `top`, `bottom`, `right`, and `left`. This is useful, when you want to do a little adjusting, but don't want to drastically alter the flow of the page. If you set `position: relative` on an element but no other positioning attributes \(top, left, bottom or right\), it will not affect the positioning at all, it will be exactly as it would be by default \(static positioning\). However, if you do give it some other positioning attribute, say, `top: 10px;`, it will shift its position 10 pixels down from where it would normally be.

## Absolute Positioning <a id="absolute-positioning"></a>

Lastly, we'll talk about absolute positioning. Add the following as the last item in your `ul`.

```text
<li><b>absolute:</b> takes element out of the normal document flow. If a parent element position is set to relative, and the child element is set to absolute, the child element's new (0,0) coordinate will be the upper left hand corner of the parent element instead of the whole page. </li>
```

Absolute position is a very powerful type of positioning that allows you to literally place any page element exactly where you want it. You use the positioning attributes top, left, bottom. and right to set the location. Remember that these values will be relative to the next parent element with relative \(or absolute\) positioning. If there is no such parent, it will default all the way back up to the `<html>` element itself meaning it will be placed relatively to the page itself.

The most important thing to remember about absolute positioning is that these elements are removed from the flow of elements on the page. An element with this type of positioning is not affected by other elements and it doesn't affect other elements. Be careful not to overuse or improperly use absolute positioning.

## Z-Index <a id="z-index"></a>

The last thing we need to talk about in terms of positioning is the `z-index`. The z-index property specifies the stack order of an element. Go ahead and put the following html below the `<ul>`.

```text
<p>The <b>z-index</b> property allows you to override the normal stacking order of the page. The default z-index is 0, and you can set that value to be positive or negative. An element with a greater z-index will stack in front of an element with a lower z-index. If two elements have the same z-index, or don't have one assigned, the element positioned last in the HTML will show on top. You must have a position assigned in order to assign a z-index. </p>
```

An element with greater stack order is always in front of an element with a lower stack order. It's important to note that the z-index only affects things with a position of absolute, relative or fixed.

## Finished Code <a id="finished-code"></a>

Your finished html and css files should look like below.

HTML:

```text
<!DOCTYPE html>
<html>
  <head>
    <title>Position</title>
    <link rel="stylesheet" type="text/css" href="08-positions.css">
  </head>
  <body>
    <div class="wrapper">
      <div class="nav">
        <p>this div has a fixed position</p>
      </div>
​
      <div class="positioning">
        <h1>Position</h1>
        <p>The position property specifies the type of positioning method used for an element. The four position values are: </p>
        <ul>
          <li><b>fixed:</b> this will pin something to a spot, and it will stay there as you scroll. (ex: nav bar) Fixed position takes elements out of the normal document flow.</li>
          <li><b>static:</b> this is the default setting, it is not affected by top, bottom, left, and right properties. It is always positioned according to the normal flow of the page.</li>
          <li><b>relative:</b> does not take the element out of normal document flow. Still appears within its space/div/container, but allows it to be offset a bit from the top, bottom, right, left. Top, right, bottom, and left properties will move it away from its normal position. Other content will not be adjusted to fit into any gap left by the element.</li>
          <li><b>absolute:</b> takes element out of the normal document flow. If a parent element position is set to relative, and the child element is set to absolute, the child element's new (0,0) coordinate will be the upper left hand corner of the parent element instead of the whole page. </li>
        </ul>
        <p>The <b>z-index</b> property allows you to override the normal stacking order of the page. The default z-index is 0, and you can set that value to be positive or negative. An element with a greater z-index will stack in front of an element with a lower z-index. If two elements have the same z-index, or don't have one assigned, the element positioned last in the HTML will show on top. You must have a position assigned in order to assign a z-index. </p>
      </div>
​
      <div class="lotsoftext">
        <h2>Here is some text, so you can scroll and see the div with a fixed position example.</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
        cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
        proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
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
.nav{
    position: fixed;
    top: 0;
    right: 0;
    width: 250px;
    background-color: lightgray;
    border: 3px solid navy;
}
​
.positioning{
    width: 75%;
    background-color: lightgray;
}
​
.positioning h1{
    text-align: center;
}
​
.lotsoftext{
    text-align: left;
    background-color: lightblue;
    width: 75%;
}
```

