# Margins & Padding

Objectives:

* Set up html and css files with css file link in head.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                03-margins-padding.css
                03-margins-padding.html
```

## Description <a id="description"></a>

Using `margin` and `padding` are ways that we can change the spacing around and between elements. The `margin` property is used to generate empty space _between_ elements, **outside** of the border, where the `padding` property that creates space _around the_ element's content **inside** of the border.

Let's grab an image from [here](https://codeleacher.files.wordpress.com/2009/04/marginandpadding.gif) to illustrate the difference between the two a little more clearly. Make sure that you save it to your `4-assets` folder with the other images saving it as margins-padding.gif so it can be referenced in the HTML as below in our example.

## Sample Code <a id="sample-code"></a>

HTML:

```text
<!DOCTYPE html>
<html>
    <head>
         <title>Margins and Padding</title>
         <!--1-->
         <link rel="stylesheet" type="text/css" href="03-margins-padding.css">
    </head>
  <body>
    <div>
      <h1>Margins and Padding</h1>
      <img src="../4-assets/marginandpadding.gif">
    </div>
​
    <!--3-->
    <div class="margins-padding">
      <h2>CSS Margins & Padding</h2>
      <h3>Margin Experiment 1</h3>
      <p id="margin-experiment1"></p>
      <p id="margin-experiment2"></p>
    </div>
​
    <br>
​
    <!--5-->
    <div class="margins-padding">
      <h3>Margin Experiment 2</h3>
      <p id="margin-experiment3"></p>
      <p id="margin-experiment4"></p>
    </div>
​
    <br>
​
    <!--7-->
    <div class="padding-class">
      <h3>Padding</h3>
      <p>Remember that padding is inside the margins and border. You can set the padding for divs, h's, p's, etc., but you will be inside the margins.</p>
​
      <h4>Padding</h4>
      <p id="padding-experiment">Here is a bunch of text to mess around with. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
      quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
      cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
      proident, sunt in culpa qui officia deserunt mollit anim id est laborum. </p>
    </div>
  </body>
</html>
```

CSS:

```text
/* 1 */
h1{
    text-align: center;
}
​
/* 4 */
.margins-padding{
  border:2px solid blue;
    margin-top: 50px;
    margin-right: 250px;
    margin-bottom: 200px;
    margin-left: 200px;
  padding: 20px 20px 20px 40px; 
}
​
#margin-demo {
    width: 400px;
}
​
#margin-experiment1{
  height: 40px;
  background: blue;
    border: 5px solid pink;
    margin: 0px 0px 0px 0px;
}
​
#margin-experiment2{
  height: 40px;
  background: blue;
    border: 5px solid pink;
    margin: 0px 0px 0px 0px;
}
​
/* 6 */
#margin-experiment3{
  height: 40px;
  background: blue;
  border: 5px solid pink;
  margin: 5px 10px 20px 0px;
  padding: 10px 10px 10px 10px;
}
​
#margin-experiment4{
  height: 40px;
  background: blue;
  border: 5px solid pink;
  margin: 5px 10px 20px 0px;
  padding: 10px 10px 10px 10px;
}
​
/* 8 */
.padding-class{
    border:2px solid red;
      margin: 50px 50px 50px 50px;
      padding: 20px 20px 20px 40px;
}
​
#padding-experiment{
    border: 2px solid yellow;
    margin: 50px 50px 50px 50px;
  /*
    padding-top: 20px;
    padding-right: 20px;
    padding-bottom: 20px;
    padding-left: 20px;
  */
    padding: 20px 20px 20px 20px;
}
```

## Discussion <a id="discussion"></a>

Now that you've got a little bit of experience with these properties, try testing different effects by uncommenting and commenting the `padding-top/right/bottom/left` in `#padding-experiment` at the bottom of your `.css` file.

## Challenge <a id="challenge"></a>

Check out the official [documentation](https://www.w3.org/TR/CSS2/box.html) on **box model** to further understand these concepts.

## Extra Resources <a id="extra-resources"></a>

​[Click here!](http://codepen.io/jamespauloconnor/pen/KMVJPE)​

