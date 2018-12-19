# iFrames

In this module we wil learn about the `<iframe>` tag.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
                14-iframe.html <---You should be here.
```

## Description <a id="description"></a>

The inline frame \(iframe\) is used to embed another document inside of an HTML document. This is a fairly straight-forward way to describe the `<iframe>`, and that is because it is a fairly straight-forward element to use in practice. Embedding third-party media is a common use of `<iframe>` and we'll show you how to insert a YouTube video into your own HTML using this tag.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>iframe</title>
</head>
<body>
​
 <iframe width="560" height="315" src="https://www.youtube.com/embed/owsfdh4gxyc" frameborder="0" allowfullscreen></iframe>       
​
</body>
</html>
```

## Discussion <a id="discussion"></a>

It may seem strange that this isn't a void element, similar to the `<img />` tag, but that is explained readily enough: compatibility with legacy versions of web browsers. If you've already tried to insert text between the opening/closing tags, you probably noticed that the text doesn't appear when the document is rendered. This is because the browser simply ignores that content. `<iframe>` can still be styled, as we have done above with the `width` and `height` attributes. However, you'll want to consider how your styling may be rendered on a variety of devices.

## Challenge <a id="challenge"></a>

Try changing the `src` attribute to a different target. How does that affect your layout? Practice changing the `width` and `height` using values such as percentages \(i.e. width="20%"\).

## Extra Reading <a id="extra-reading"></a>

Resources: [http://html.com/tags/iframe/](http://html.com/tags/iframe/)​

