# Inputs

In this module we will do the following:

1. Understand the `<input />` tag.
2. Discuss empty tags.
3. Describe two ways to write an input tag. With and without a /.
4. Create two more input fields.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
                08-input.html <---You should be here.
            └── CSSPrework
            └── PythonPrework
            └── assets
```

## Description <a id="description"></a>

Input tags are one of several element types that allow users to interact with your website. Their use is probably self-explanatory, but for clarity let's just say that the `<input />` tag provides an empty field which can be filled with text. You may have noticed that `<input/>` doesn't have a mated closing tag. Much like `<br />` or `<hr />`, this tag is an "empty" element. You may see empty elements referred to as "void" or "self-closing". All of these terms mean roughly the same thing: they don't require a closing tag. The reason for this is that the entire element is described by a single tag. These elements may not contain additional content, which also means that you can't nest a `<div></div>` or any other element inside of them. **However**, they may have attributes, such as a `class` or `id` for purposes such as styling.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
    <head>
        <title>Input</title>
</head>
<body>
    <h1>Input Tag</h1>
    <p>Name</p><input />
    <p>Email</p><input>
</body>
</html>
```

## Discussion <a id="discussion"></a>

As mentioned, the input tag is ubiquitous. It's important to identify that when we describe it using HTML, the browser merely renders a _location_ for input to be placed. To actually capture the information that users insert requires the use of JavaScript. Another detail worth clarifying is a difference you may have noticed when writing this code: one of the inputs is written as `<input />`, while the other is written as `<input>`. What's with the difference, and why do they both still work? The explanation is simply that empty elements do not **require** a closing `/`. HTML5 is smart enough to know what's going on. However, it is worth noting that it's good practice to close all of your elements for the sake of specificity. Programming with intention is a hallmark of a great developer.

## Challenge <a id="challenge"></a>

Now that you have a pretty good grasp on applying `<input />`, try making two new fields marked as 'address' and 'cc number'. Try shifting the elements around to see how they are rendered differently.

