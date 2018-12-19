# CSS Setup

Objectives:

1. Review `HTML`
2. Set up a link to the `CSS` file in HTML head.
3. Set up a simple wrapper.

## File Location <a id="file-location"></a>

For this lesson you'll be working in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework <-- should be done
            └── CSSPrework
                00-setup.css
                00-setup.html
                01-classes.css
                01-classes.html
                02-ids.css
                02-ids.html
                03-margins-padding.css
                03-margins-padding.html
                04-fonts.css
                04-fonts.html
                05-backgrounds.css
                05-backgrounds.html
                06-widths-heights.css
                06-widths-heights.html
                07-borders.css
                07-borders.html
                08-positions.css
                08-positions.html
```

## Description <a id="description"></a>

`CSS` \(Cascading Style Sheets\) is the language we use to tell the browser what elements in our `HTML` document _should look like_. It's common to hear HTML described as the skeleton of our document and CSS described as the skin. This is because HTML defines where elements are rendered, and CSS defines the characteristics of those elements.

Using the `id` and `class` attributes, we can use CSS to target a single specific element \(`id`\), or apply a style to all of the elements of a group \(`class`\).

You can use CSS to do the following:

1. Give the outside of the site a unique look and feel.
2. Alter colors, fonts, backgrounds, etc.
3. To implement some effects and light animations.

In the sample code, note that we're using a `<link>` tag inside of the `<head>` to tie a CSS file to our HTML. This is done in the `<head>` so that the browser will load the CSS file before it renders the HTML elements. Because the browser reads line-by-line, if we loaded the CSS file at the bottom of the page, then the HTML will have already rendered and the result may be a negative experience for our users. This is especially evident on a slow connection, because all of the processes \(including loading CSS\) _simply take longer_ to make their way down the wire.

At this point, let's go ahead and grab another image to visualize how a `.css` statement is written. Go [here](http://djnmarti.com/foothill/coin65/week_02/images/anatomy_css_rule.gif) and save the image to your `4-assets` folder.

## Sample Code <a id="sample-code"></a>

```text
<!DOCTYPE html>
<html>
  <head>
    <title>CSS Notes</title>
    <link rel="stylesheet" type="text/css" href="00-setup.css" />   
  </head>
  <body>
  <h1>CSS Notes</h1>
    <div class="wrapper">
      <h2>CSS Statements</h2>
      <p>Four main components include the following: </p>
      <ol> 
        <li><b>Declaration: </b>the statement as a whole with curly braces.</li> 
        <li><b>Selector:</b> the name of the part you want to style.</li>
        <li><b>Property:</b> properties to edit(e.g., width, height, background, etc.)</li>
        <li><b>Value:</b> numbers, colors, urls - values that we assign. </li>
      </ol>
      <p>Here's a photo to illustrate these items:</p>
      <img src="../4-assets/anatomy_css_rule.gif" id="css-photo" >
    </div>
  </body>
</html>
```

In the above code, we've assigned a `class`.

## Adding CSS <a id="adding-css"></a>

In the `00-setup.css` file, add the following code:

```text
body {
    background-color: #D3D3D3;
}
.wrapper {
    border: 10px solid red;
}
```

You should see a different background color, and you should see an awesome red border after you save both files and load the HTML to your browser.

## Comments in CSS <a id="comments-in-css"></a>

Here's how to do a comment in CSS:

```text
/*This is a CSS comment*/
body {
    background-color: #D3D3D3;
}
/*This is another CSS comment*/
.wrapper {
    border: 10px solid red;
}
```

## Discussion <a id="discussion"></a>

In this lesson, we've introduced the concepts of `class` and `id`, as well as shown how \(and just as importantly, **why**\) to add a CSS file to the head of an HTML document. We've also made you aware of `class` and `id`, which we'll explore in greater depth in the following lessons.

## Challenge <a id="challenge"></a>

Investigate hex colors [here](https://htmlcolorcodes.com/color-picker/) and try changing the `background-color` attribute that you defined in the `.css` file. Experiment with the `border` attribute in the `.wrapper` selector.

