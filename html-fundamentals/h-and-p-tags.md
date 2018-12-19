# H & P Tags



In this module we'll start to study some of the most commonly used tags in HTML. Here are the module objectives:

1. Discussion of h & p tags with a few examples.
2. Show descending h tags.
3. Show hr & br tags for organizing.
4. Run browser and show completed Two Truths, One Lie game.
5. Recreate step 4 with own details.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
Python_Projects
└──prework
    └──HTMLPrework
        02-h&p-tags.html
```

## Start Code

Get started with by adding the following code to the file. Helpful tip: To get the starting structure for an HTML page, type `!` then `tab`. It should scaffold out the html code:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Two Truths, One Lie</title>
</head>
<body>​
</body>
</html>
```

## Example Code

Let's start with the `h` tag. This is probably the most used tag. `h` defines html **headings**, and there are 6 different sizes. Add the following code to the file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Two Truths, One Lie</title>
</head>
<body>
​
    <h1>H1 Tag</h1>
    <h2>H2 Tag</h2>
    <h3>H3 Tag</h3>
    <h4>H4 Tag</h4>
    <h5>H5 Tag</h5>
  <h6>H6 Tag</h6>
​
</body>
</html>
```

After running the code, you should see 6 different sizes of heading tags in your browser window.

## p Tags <a id="p-tags"></a>

Another extremely common tag is the `p` tag. A `p` tag defines a **paragraph** and has some default settings for paragraphs on it:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Two Truths, One Lie</title>
</head>
<body>
  <h1>h1 Tag</h1>
    <h2>h2 Tag</h2>
    <h3>h3 Tag</h3>
    <h4>h4 Tag</h4>
    <h5>h5 Tag</h5>
  <h6>h6 Tag</h6>
​
  <p>Here is a p tag. This will be for things like paragraphs. </p>
</body>
</html>
```

## Two Truths One Lie <a id="two-truths-one-lie"></a>

Here's a task to get you some more practice with HTML. Create a Two Truths, One Lie HTML page about yourself.

```text
<!DOCTYPE html>
<html>
<head>
    <title>Two Truths, One Lie</title>
</head>
<body>
  <!-- Add this below the code you previously added -->
    <h1>Two Truths, One Lie</h1>
    <p>Overview: Here are some notes for the Two Truths, One Lie about me. Good luck figuring it out! You never will!</p>
​
    <hr />
​
    <h2>Japan</h2>
    <p>I visit Japan once a year for a tech conference.</p>
​
    <h2>Steve Jobs</h2>
    <p>I worked with Steve Jobs when I was younger.</p>
​
    <h2>Crime Watch</h2>
    <p>I wrote a Crime Watch mobile app that helps police spot criminal behavior.</p>
</body>
</html>
```

## Final Code <a id="final-code"></a>

```text
<!DOCTYPE html>
<html>
<head>
    <title>h, p, & hr tags</title>
</head>
<body>
​
  <h1>H1 Tag</h1>
    <h2>H2 Tag</h2>
    <h3>H3 Tag</h3>
    <h4>H4 Tag</h4>
    <h5>H5 Tag</h5>
  <h6>H6 Tag</h6>
​
  <p>P Tag</p>
​
  <hr />
  <br />
  <br />
  <br />
​
  <h1>About Me</h1>
    <p> Hello, I am happy to be here.</p>
    <hr />
    <h1>More about me</h1>
    <p> Here's some more info about me.</p>
​
    <h1>Two Truths, One Lie</h1>
    <p>Overview: Here are some notes for the Two Truths, One Lie about me. Good luck figuring it out! You never will!</p>
​
    <hr />
​
    <h2>Japan</h2>
    <p>I visit Japan once a year for a tech conference.</p>
​
    <h2>Steve Jobs</h2>
    <p>I worked with Steve Jobs when I was younger.</p>
​
    <h2>Crime Watch</h2>
    <p>I wrote a Crime Watch mobile app that helps police spot criminal behavior.</p>
​
</body>
</html>
```



