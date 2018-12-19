# Links

In this module we will do the following:

1. Describe `href` and using links. Discuss the `<a></a>` tag.
2. Study different ways to hyperlink. \(internal and external\)

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
                04-links.html <---You should be here.
            └── 2-CSS-Basics
```

## Anchor Tags <a id="anchor-tags"></a>

An anchor is a piece of text that marks the beginning and end of a hypertext link. It is indicated in HTML using the `<a></a>` tag and will display text between the opening and closing tags as the standard, blue, underlined [link](https://eleven-fifty-academy.gitbook.io/dotnet-100-prework-gitbook/part-1-html-fundamentals/links) that you have probably become accustomed to seeing.

### Hrefs <a id="hrefs"></a>

Within an `<a>` tag, you commonly add a `href` which allows you to direct the link to the url or local path you want to go. Common syntax for this is `<a href="www.google.com">Google</a>`.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
​
        <h1>The anchor tag</h1>
        <p>This tag is used for hyperlinking internally and externally.
​
        <h3>Linking to a URL</h3>
        <a href="https://efa-lms-e8982.firebaseapp.com/home">Eleven Fifty LMS</a>
​
        <h3>Linking to local html file</h3>
        <a href="01-basic-tags.html">Basic Tags page</a>
​
        <h3>Click the link to open another window</h3>
        <a href="https://efa-lms-e8982.firebaseapp.com/home" target="blank">Eleven Fifty LMS</a>
​
    </body>
</html>
```

## Targets <a id="targets"></a>

When you run your code using `alt + b`, all of the links that appear on your browser page should be functional. Clicking on them will navigate you to other places. Notice though, there is a slight difference between the first and third example: target="blank" is what causes the link to be opened in a new tab when you click on it.

## Relative paths <a id="relative-paths"></a>

In the second example above, you wrote an `<a></a>` tag that linked to a local file. To do this, we used "relative pathing". This is an important concept that is used very frequently during development. For now, just recognize that you are connecting this .html file with another .html file.

## Challenge <a id="challenge"></a>

Now that you've got examples of different ways to write anchor tags, see if you can write a few that link to some of your favorite web pages!

