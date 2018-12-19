# Fonts

Objectives

* Discuss font.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                04-fonts.css
                04-fonts.html
```

## Description <a id="description"></a>

Font changes impact the experience a user has on your site. Choosing the right font, size, color, and styling can drastically effect the enjoyability of your app.

Let's have you build out the files necessary to incorporate these styles:

```text
<!--1-->
<!DOCTYPE html>
<html>
  <head>
    <title>Font</title>
    <link rel="stylesheet" type="text/css" href="04-fonts.css">
  </head>
  <body>
    <div class="wrapper">
      <!--2-->
      <h1>Font</h1>
      <p>In CSS, there are two types of font family names:</p>
      <ul>
        <li><b>generic family:</b> a group of font families with a similar look (ex: Serif)</li>
        <li><b>font family:</b> a specific font family (ex: "Times New Roman" or Arial)</li>
      </ul>
      <p>The font-family property should hold several font names as a fallback in case the browser doesn't support the first font you picked. <br>Always start with the font you want, and end with a generic family. Also, if the font family is more than one word, it must be in <br>quotation marks (ex: "Times New Roman").</p>
​
      <hr>
​
      <!--3-->
      <h2>Here is a list of the CSS font properties:</h2>
      <dl>
        <dt>font:</dt>
        <dd>sets all the font properties in one declaration</dd>
        <dt>font-family:</dt>
        <dd>specifies the font family for text</dd>
        <dt>font-size:</dt>
        <dd>specifies the font size of text</dd>
        <dt>font-style:</dt>
        <dd>specifies the font style for text</dd>
        <dt>font-weight</dt>
        <dd>specifies the weight of a font</dd>
      </dl>
​
    <hr>
​
    <!--5-->
    </div>    
  </body>
</html>
```

```text
.wrapper{
    margin: 5px;
}
​
/* 4 */
​
p{
    font-family: "Times New Roman", Times, serif;
}
​
h2{
    font-family:Arial, Helvetica, sans-serif;
}
​
dt{
    font-weight: bold;
    font-size: 20px;
}
```

## Discussion <a id="discussion"></a>

As you can see there's a lot to unpack regarding `font`. Another method includes loading fonts from other sources \(such as [Google Fonts](https://fonts.google.com/)\). Probably the single most important thing to take away from this lesson is the redundancy that is necessary when designing for a variety of browsers.

Having fallback fonts for when a browser doesn't support the most desirable one is your first introduction to redundancy and planning for worst-case scenario in development. You will discover that this theme is revisited from a variety of directions during your growth as a developer.

## Challenge <a id="challenge"></a>

If you'd like more examples of different font properties, [here](http://www.w3schools.com/css/css_font.asp) is a link.

If you'd like to learn more about font families, [here](http://www.w3schools.com/cssref/css_websafe_fonts.asp) is a link to commonly used font combinations.

