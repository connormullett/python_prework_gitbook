# Ids

Objectives:

1. Set up html and css files with css file link in head.
2. Test set up with a color change: body { background-color: blue; }
3. Reveal info about ids.
4. Show difference between ids and classes.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    DotNetProjects        └── HTMLCSSPreWork            └── 1-HTML-Basics            └── 2-CSS-Basics                02-ids.css                02-ids.html
```

## Description <a id="description"></a>

The `id` attribute is a **unique** identifier. Where a `class` attribute can be applied to many different elements, an `id` points to only _one_ element. This allows you to manipulate that particular element without worrying about affecting anything else.

Furthermore, an `id` takes precedent over `classes`. If, for example, you have conflicting CSS styling on a particular element, one under a class element and the other under an id, the `id` attribute will be used. This allows you to prioritize your styling and, if needed, overrule generalized styling of your app.

## Sample Code <a id="sample-code"></a>

```text
<!DOCTYPE html>
<html>
  <head>
    <title>CSS ids</title>
    <link rel="stylesheet" type="text/css" href="02-ids.css">
  </head>
  <body>
    <h1>CSS ids</h1>
    <p>An ID is a UNIQUE identifier </p>
    <div>
      <h3>id notes</h3>
      <ul> 
        <li>start with a pound - #</li>
        <li>uses: header or an about section</li>
        <li>Should only be used once per page - they are unique! Important with JavaScript later on.</li> 
        <li>Use for one off styling.</li>
      </ul>
    </div>
    <div>
      <h1>Ids versus Classes</h1>
      <h2>Ids</h2>
      <p id="number-one">This id will be linked in the CSS page by a #</p>
      <p id="number-one number-two">You can't have two ids on an element.</p>
​
      <h2>Classes</h2>
      <p class="first-class">one class here.</p>
      <P class="first-class second-class">Two classes here.</P>
​
      <p id="number-one" class="first-class">You CAN use an id twice, but you shouldn't.</p>
    </div>        
  </body>
</html>
```

## Sample Code <a id="sample-code-1"></a>

CSS:

```text
/* For Testing */
/*body {
    background-color: blue;
}*/
​
#number-one{
    color: red;
}
​
#number-two{
    font-size: 16px;
}
​
.first-class{
    color: green;
}
​
.second-class{
    font-size: 24px;
}
```

## Discussion <a id="discussion"></a>

Having the knowledge of classes under our belts, we can examine the uses of `id`. When we want to target several elements, `class` is the right choice. If we're trying to target a single element, that's when `id` is preferable. In our above example, we've shown not only how to target with an `id`, but also proven that multiple classes can be assigned to a single element. Finally, it's important to recognize that our very last `<p>` has both an `id` **and** a `class`!

Take note of the detail that when a `property` is assigned a conflicting `value` in both an `id` and a `class`, such as our `#number-one` and `.first-class`, the `id` has preference. In the case of our example, this means that `color` receives the `value` of "red".

## Challenge <a id="challenge"></a>

Experiment with `id`, and try testing new properties.

