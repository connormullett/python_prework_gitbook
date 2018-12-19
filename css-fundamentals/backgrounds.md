# Backgrounds

Objectives:

* Discuss the `background` property.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                05-backgrounds.css
                05-backgrounds.html
```

## Description <a id="description"></a>

You've probably already guessed what `background` does; it changes the field upon which the content of an HTML element resides in.

Let's go ahead and grab a cool picture to use as a background. Go [here](http://atelierkarim.com/assets/grfx/site/backgrounds/upfeathers.png) and save the image in your `4-assets` folder, with the rest of your resources.

## Sample Code <a id="sample-code"></a>

Let's add this sample code to your `background.html` file:

```text
<!DOCTYPE html>
<html>
  <head>
    <title>Backgrounds</title>
    <!--1-->
    <link rel="stylesheet" type="text/css" href="05-background.css">
  </head>
  <body>
    <div class="wrapper">
​
      <!--2-->
      <h1>Background</h1>
      <p>You can set the background of your webpage to a simple color, or you can use an image. The background you set can be for the entire page and/or certain divs. </p>
​
      <hr>
​
      <!--4-->
      <div class="background1">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
      proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
​
    <hr>
​
    <!--5-->
    <div class="background2">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
      proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
​
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
      proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
​
      <!--6-->
      <table>
        <tr>
          <th>First Name</th>
          <th>Last Name</th>
          <th>Occupation</th>
        </tr>
        <tr>
          <td>Sherlock</td>
          <td>Holmes</td>
          <td>Consulting Detective</td>
        </tr>
        <tr>
          <td>John</td>
          <td>Watson</td>
          <td>Doctor</td>
        </tr>
      </table>
    </div>
  </body>
</html>
```

## CSS Sample Code <a id="css-sample-code"></a>

Let's add this sample code to your `background.css` file:

```text
.wrapper{
    margin: 5px;
}
​
/* 3 */
h1{
    text-align: center;
}
/*this sets the background color of the entire body*/
body{
    background-color: lightgray;
}
​
/* 4 */
.background1{
    background-color: lightblue;
}
​
/* 5 */
.background2{
    background-image:url("../4-assets/upfeathers.png");
}
​
/* 7 */
table, th, td{
    border: 1px solid black;
}
```

## Discussion <a id="discussion"></a>

Much like fonts, backgrounds are another aspect of an application that can make or break the user experience. You can see that implementing `background` isn't as challenging as many other properties, however, consider carefully what the result will be. Neutral colors, grayscales and blurred backgrounds tend to be more accessible to the average user.

It's important to note how the file path works here: `../4-assets/upfeathers.png`. When we use `../`, that means back up one level from the current directory, then, go look for the `4-assets` folder. Inside there, look for `upfeathers.png`. If we wanted to look two directories above, we could say `../../`.

## Challenge <a id="challenge"></a>

Find an image you like, and try using it as a `background`. Explore other options like [gradients](https://www.w3schools.com/css/css3_gradients.asp) as backgrounds.

