# Images

In this module we will do the following:

1. Discuss the image \(`<img>`\) tag.
2. Set up an image folder and place an image in the folder.
3. Create reference to an image.
4. Find a URL for an image and use it.
5. Resize the image w/ basic inline styling.
6. Create a hyperlink from an image.
7. Add a few more images with favorite places or things. Use a variety of links and styling.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
                05-images.html <--- here
```

## Description: <a id="description"></a>

Images are defined with `img` tags and do not have a closing tag. Like `hr` and `br`, they are self-closing tags.

## Image Folder <a id="image-folder"></a>

For this module, you'll be adding a new folder to your project to contain images. This is another example of relative pathing, which was briefly discussed on the "Links" page. For ease of reference, we'll be adding this folder to the same directory as HTML, CSS, and JS Basics. Name the folder 4-assets. Your new folder structure should look like this:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
            └── PythonPrework
            └── Assets
```

## Adding Assets <a id="adding-assets"></a>

Great! Now that we've added the folder to contain our pictures, let's go get some assets to use on our website. Using your browser, navigate to [https://ericjoyner.com/turnfortheworse/](https://ericjoyner.com/turnfortheworse/) and right click on the artwork you're presented with. Choose "Save image as..." from the list that appears, and save the image to the 4-assets folder we just created.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Images</title>
</head>
<body>
​
    <h3>Image referenced from inside the project</h3>
    <img src="../4-assets/TurnForTheWorse.jpg" width="300" height="300">
​
    <hr>
    <h3>Referencing an outside URL</h3>
    <img src="http://www.ufunk.net/wp-content/uploads/2012/01/retro-robot-donut-eric-joyner-01.jpg">
​
    <hr>
​
    <h3>Image referencing another page from an image</h3>
    <a href="https://ericjoyner.com/turnfortheworse/"><img src="../4-assets/TurnForTheWorse.jpg" width="300" height="300">
    </a>
​
    <hr>
​
    <h3>Adding a little style to the image</h3>
    <a href="https://ericjoyner.com/turnfortheworse/"><img src="../4-assets/TurnForTheWorse.jpg" class="circle" width="300" height="300">
    </a>
​
    <style>
    .circle{
        border-radius: 150px;        
    }
​
    </style>
​
</body>
</html>
```

## Self-Closing Tags <a id="self-closing-tags"></a>

Here we have a few tags for organizing concepts. They are not as common, but useful to know about. They also can teach us about self-closing tags. Self-Closing tags only have one tag involved. They are open and closed. We can write them like this: `<hr />` or `<hr>`

`hr` Stands for **horizontal rule**: Used to separate content. Provides a horizontal line between items. `br` Is simply a line **break**: separates content using white space instead of a line. \(We used one here, to prevent the sentence about `br` from wrapping up to the line above!\)

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
</body>
</html>
```

## Discussion <a id="discussion"></a>

So, let's dig into what's going on in this file a little bit: In the first example, we're referencing a location inside our project using relative pathing in the `src` attribute. In this case, we back up one step \(`../`\) in the directory tree and then dive into our `4-assets` folder \(`4-assets`\), which would look like `../4-assets`; and then point directly at the image we want to be displayed \(`/TurnForTheWorse.jpg`\). The entire path that you type out should look like this: `../4-assets/TurnForTheWorse.jpg`. In the other examples, we've nested `<img>` tags inside of `<a>` tags so that the images themselves act as links. The final example uses the `class` attribute and the `<style>` tag \(more on this soon\) to display our picture as a circle.

```text
Python_Projects
    └── prework
        └── HTMLPrework
        └── CSSPrework
        └── PythonPrework
        └── Assets
            └── TurnForTheWorse.jpg
```

## Challenge <a id="challenge"></a>

Now that you've got a grasp on how this tag works, try to incorporate one of your own pictures. Save your image to your assets folder and experiment!

