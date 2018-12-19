# Articles & Headers

In this module we will do the following:

1. Discuss headers.
2. Create a basic header with minimal styling.
3. Discuss articles.
4. Discuss how headers can be used and more easily recognized and manipulated in these articles and sections.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
     Python_Projects
        └── prework
            └── HTMLPrework
                11-articles-headers.html <---You should be here.
```

## Article <a id="article"></a>

"The article element represents a component of a page that consists of a self-contained composition in a document, page, application, or site and that is intended to be independently distributable or reusable, e.g. in syndication. This could be a forum post, a magazine or newspaper article, a blog entry, a user-submitted comment, an interactive widget or gadget, or any other independent item of content." [Attribution](https://html5doctor.com/the-article-element/) for the above statement.

## Headers <a id="headers"></a>

Headers are containers for other informational elements and act as a title for the element that they are contained within. Headers are **not** the same as _headings_.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html><html><head>    <title>Articles and Headers</title></head><body>​<h1>Header tag notes</h1><ul>  <li>Can be the beginning of any section. Not just top of page.</li>  <li>Semantic element that lets us know where a section begins.</li>  <li>Allows you to more easily style the headers of a section.</li></ul>​<header style="width:100%; text-align:center; background-color:pink;">  <h1>Dang Good Donuts</h1></header>​​<h1>Article tag notes</h1><ul>    <li>Use in posts</li>    <li>Independent content</li>    <li>RSS feed</li>    <li>Content makes sense on its own when everything else is gone.</li>    <li>Specialized kind of section</li></ul>​​<hr>​<header style="width:100%; text-align:center; background-color:pink;">  <h1>Doug's Dang Good Donuts</h1></header>​<section style="width:70%; float: left; background-color: blue;">        <header style="text-align:center;">        <h3>Welcome to the Donut Store</h3>        </header>          <p>          Lorem ipsum cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o. Ice cream cake powder.          Dragée cheesecake cupcake cheesecake danish toffee. Jujubes gummi bears fruitcake candy canes. Candy canes toffee candy icing carrot cake. Marzipan gummies sesame snaps chocolate wafer jelly beans biscuit gummies chupa chups.          Candy canes danish tart wafer cupcake soufflé jelly pie. Chocolate jujubes danish pie jelly candy canes chocolate cake. Pastry icing tiramisu gingerbread caramels croissant bear claw lollipop.          Cotton candy candy canes cookie tiramisu sugar plum muffin biscuit lollipop. Marzipan topping chocolate bar wafer jelly-o.           </p></section>​<article style="width: 30%; float: right; background-color: gray;">      <header style="text-align:center; color: purple;">          <h2>The Jelly-Filled Nightmare</h2>      </header>      <section>          <h4>Original Reviewer</h4>              <p>That donut was so great!</p>              <p>Posted on <time datetime="2015-05-15 19:00">May 16</time> by Paul.</p>          <h4>Replies</h4>              <p>Way too sugary for me.</p>              <p>Posted on <time datetime="2015-05-16 19:00">May 16</time> by Auri.</p>              <p>I agree, the donut was great. Auri is weak!</p>              <p>Posted on <time datetime="2015-05-17 19:00">May 17</time> by Jonas.</p>      </section></article>​</body></html>
```

## Discussion <a id="discussion"></a>

So, in the description we quoted it was stated that `<article>` is used for any "independent item of content". What does that mean? Basically, if you're able to strip away all of the content from around the `<article>Content</article>` and it still makes sense, then it might belong in an `<article>`! We're introducing `<header>` in this same lesson because these two elements are frequently seen together. You'll see this pattern because stand-alone content \(like an article, right?\) tends to need ways to identify the content for the user. Briefly, it's worth remarking that the `<header>` element is **not** the same as a _heading_ tag like an `<h2></h2>`. Much like the title to a book, `<header>` acts as a container for introductory content like a _heading_ or a logo.

## Challenge <a id="challenge"></a>

Check out the attributes on the two bottom-most articles. There's some inline-styling present. Try changing the `float` and `width` parameters and observe how it changes what's rendered to the browser. Experiment fearlessly and add new articles with elements of your choosing.

