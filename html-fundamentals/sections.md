# Sections

In this module we will do the following:

1. Explanation of sections.
2. Create a section that covers the entirety of the page, has a heading, and some text.
3. Customize with some basic inline CSS.
4. Create two sections side by side, using a little CSS.
5. Discuss the difference between div and section

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
   Python_Projects
        └── prework
            └── HTMLPrework
                10-sections.html <---You should be here.
```

## Description

Sections are like divs, but they are semantic groupings. They help the browser and the developer understand that there is a particular grouping coming. The `<section>` tag defines sections in a document, such as chapters, headers, footers, or any other sections of the document.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
    <head>
        <title>Sections</title>
    </head>
    <body>
​
        <h1>BRONZE</h1>
        <section>
            <h3>Welcome to the Donut Store</h3>
                <p>
                Lorem ipsum cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. Ice cream cake powder.
                Dragée cheesecake cupcake cheesecake danish toffee. Jujubes gummi bears fruitcake candy canes. Candy canes toffee candy icing carrot cake. Marzipan gummies sesame snaps chocolate wafer jelly beans biscuit gummies chupa chups.
                Candy canes danish tart wafer cupcake soufflé jelly pie. Chocolate jujubes danish pie jelly candy canes chocolate cake. Pastry icing tiramisu gingerbread caramels croissant bear claw lollipop.
                Cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. 
                </p>
        </section>
​
        <h1>SILVER</h1>
        <section style="width:50%; background-color: green;">
            <h3>Welcome to the Donut Store</h3>
                <p>
                Lorem ipsum cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. Ice cream cake powder.
                Dragée cheesecake cupcake cheesecake danish toffee. Jujubes gummi bears fruitcake candy canes. Candy canes toffee candy icing carrot cake. Marzipan gummies sesame snaps chocolate wafer jelly beans biscuit gummies chupa chups.
                Candy canes danish tart wafer cupcake soufflé jelly pie. Chocolate jujubes danish pie jelly candy canes chocolate cake. Pastry icing tiramisu gingerbread caramels croissant bear claw lollipop.
                Cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. 
                </p>
        </section>
​
        <br>
        <br>
​
        <h1>GOLD</h1>
        <section>
            <section style="width:70%; float: left; background-color: red;">
                <h3>Welcome to the Donut Store</h3>
                    <p>
                    Lorem ipsum cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. Ice cream cake powder.
                    Dragée cheesecake cupcake cheesecake danish toffee. Jujubes gummi bears fruitcake candy canes. Candy canes toffee candy icing carrot cake. Marzipan gummies sesame snaps chocolate wafer jelly beans biscuit gummies chupa chups.
                    Candy canes danish tart wafer cupcake soufflé jelly pie. Chocolate jujubes danish pie jelly candy canes chocolate cake. Pastry icing tiramisu gingerbread caramels croissant bear claw lollipop.
                    Cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. 
                    </p>
            </section>
            <section style="width:30%; float: right; background-color: yellow;">
                <h3>Another section</h3>
                    <p>
                    Lorem ipsum cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. Ice cream cake powder.
                    Dragée cheesecake cupcake cheesecake danish toffee. Jujubes gummi bears fruitcake candy canes. Candy canes toffee candy icing carrot cake. Marzipan gummies sesame snaps chocolate wafer jelly beans biscuit gummies chupa chups.
                    Candy canes danish tart wafer cupcake soufflé jelly pie. Chocolate jujubes danish pie jelly candy canes chocolate cake. Pastry icing tiramisu gingerbread caramels croissant bear claw lollipop.
                    Cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. 
                    </p>
            </section>
        </section>
    </body>
</html>
```

## Discussion <a id="discussion"></a>

Introduced in HTML5, the `section` tag is helpful in allowing us to avoid 'divitis'. Having a variety of ways to separate our code is useful, but the real advantage is that content inside `<section>` is grouped to indicate a common theme. A `<section>` is usually indicated by a heading \(`<h1>-<h6>`\) as a nested or **child** element. This contrasts with `<div>` where the elements contained within it are only related by being children of the `<div>` and by `attributes` assigned to the `<div>`. This is another example of intentional programming in that an unaware, or apathetic, developer may sling `<div>` tags around with no recognition for the superior accessibility to screen readers and easier maintainability for authors that `<section>` offers.

## Challenge <a id="challenge"></a>

Experiment with the sections you just made, changing the inline styling or adding other elements to the document.

## Extra Reading <a id="extra-reading"></a>

​[This](https://www.w3.org/TR/html/sections.html#the-section-element) is an excellent resource from the team that defines the standards that the internet operates by. Start getting into the habit of looking for information from first-party sources and the authors of the technology that we all use.

