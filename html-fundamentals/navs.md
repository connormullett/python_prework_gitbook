# Navs

In this module we will discuss the `<nav>` tag.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
     Python_Projects
        └── prework
            └── HTMLPrework
                13-nav.html <---You should be here.
```

## Description: <a id="description"></a>

The `<nav>` tag is typically used to collect a set of navigation links. This is not intended to suggest that **every** link in your application should be encapsulated inside of a `<nav>`. The links collected in a `<nav>` are usually used to traverse through different pages in your application, usually in a navbar at the top of your application.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Nav</title>
</head>
<body>
    <div>
        <nav>
          <a href="/html/">HTML</a>
          <a href="/css/">CSS</a>
          <a href="/js/">JavaScript</a>
        </nav>
    </div>
​
    <nav>
        <h1>Vertical Navigation Bar</h1>
            <ul>
                <li><a href="03-lists.html">Lists</a></li>
                <li><a href="05-images.html">Images</a></li>
                <li><a href="06-tables.html">Tables</a></li>
            </ul>
    </nav>
​
    <footer>
    <p>Copyright © 2006 The Example Company</p>
    <p><a href="about.html">About</a> -
    <a href="policy.html">Privacy Policy</a> -
    <a href="contact.html">Contact Us</a></p>
    </footer>
​
</body>
</html>
```

## Discussion <a id="discussion"></a>

We've provided two examples above, but there are innumerable ways to accomplish this task, and the needs of the application may demand a specific solution. The first example is typical and produces a horizontally-aligned navbar. In the second example, we've specified that the browser should render the navbar vertically as an unordered list by using `<ul>` and `<li>` tags.

## Challenge <a id="challenge"></a>

Try adding new links to your navbar. Experiment with the `href` attribute and try navigating to an outside webpage. Try adding an attribute to keep your webpage open and open the linked page in a new tab. Check out the code in [lesson 4](https://eleven-fifty-academy.gitbook.io/dotnet-100-prework-gitbook/part-1-html-fundamentals/links) if you need a refresher.\(hint: it's in the "target" portion of the lesson\)

## Extra Reading: <a id="extra-reading"></a>

​[http://www.html-5-tutorial.com/nav-element.htm](http://www.html-5-tutorial.com/nav-element.htm)​

