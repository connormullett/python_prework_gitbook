# Basic Tags



In this module, we'll discuss the following:

1. Basic tags, especially head & body.
2. Create a basic Hello World page

## File Location <a id="file-location"></a>

You should be located in the following file:

```text
 Python_Projects
  └── prework
   └── HTMLPrework              
       01-basic-tags.html <-----You should be here
```

## Tags <a id="tags"></a>

A tag is used to surround content and apply meaning. The opening tag tells the browser to start _rendering_ something. The closing tag tells the browser where the tag ends.

## Starter Code <a id="starter-code"></a>

While inside your `01-basic-tags.html`, add the following code:

```text
<!DOCTYPE html>
<html>    
    <head>​    
    </head>    
    <body>        
        <h1>Hello World</h1>    
    </body>
</html>
```

Notice that there is a closing tag for each opening one. For instance, `<h1>` is closed by `</h1>`. The `/` indicates closing. So everything within those two tags will be shown in the browser.

Let's break down a few of the tags in the above code:

## DOCTYPE <a id="doctype"></a>

`DOCTYPE` states the document type. It's a declaration that lets the browser know which flavor of html you are using. For our purposes in this course, we will always use this tag to start our `html` pages.

## `<html>The HTML Tag</html>` <a id="less-than-html-greater-than-the-html-tag-less-than-html-greater-than"></a>

`html` hypertext markup language is language used for describing web documents. All of our HTML code will get nested inside of there.

## `<head>The Head Tag</head>` <a id="less-than-head-greater-than-the-head-tag-less-than-head-greater-than"></a>

The `<head>` element is a container for metadata \(data about data\) and is placed between the `<html>` tag and the `<body>` tag. Nothing in the head will show up on the page, except for the . Except for using a `<title>` tag, contents inside the head tag are not visible on the page.

## `<title>The Title Tag</title>` <a id="less-than-title-greater-than-the-title-tag-less-than-title-greater-than"></a>

The `<title>` tag is required in all HTML documents, and it defines the title of the document.

1. Defines a title in the browser toolbar
2. Provides a title for the page when it is added to favorites
3. Displays a title for the page in search-engine results

```text
<!DOCTYPE html><html>    <head>    <!-- Add title here -->        <title>Hello World</title>    </head>    <body>        <h1>Hello World</h1>    </body></html>
```

An example: ![title](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAU8YfAhlshtlbw2DNJ%2F-LBuvSNs0gUVOgjXIE5Z%2F-LBuvZo8vwp1dXJqWc99%2Ftitle.PNG?generation=1525702087367352&alt=media)​

## `<body>The Body Tag</body>` <a id="less-than-body-greater-than-the-body-tag-less-than-body-greater-than"></a>

The body tag defines a document's body. Items placed inside of the body tag will render to the DOM\(the Document Object Model\) and be seen in the view.

## Consider This: <a id="consider-this"></a>

Think of the head as doing the invisible thinking and setup; the body manifests or shows the actual content.

## Run the Code <a id="run-the-code"></a>

Now that you've added some HTML, let's run the code. 1. Save your file by pressing `ctrl + s` \* 2. On a Windows machine, click on the `.html` file and press `ctrl + alt + o`. On a Mac `cmd + alt + o`. 3. You should be given a list of browsers. Choose Chrome.

## 

