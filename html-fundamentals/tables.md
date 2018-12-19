# Tables

In this module we will do the following:

1. Discuss the `<table>` tag.
2. Show a simple table with no styling.
3. Add a small amount of styling.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text
 PythonProjects
        └── prework
            └── HTMLPrework
​
                06-tables.html <---You should be here.
```

## Description <a id="description"></a>

An HTML table is defined with the `<table>` tag. Each table row is defined with the `<tr>` tag. A table header is defined with the `<th>` tag. By default, table headings are bold and centered. A table data/cell is defined with the `<td>` tag.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Tables</title>
</head>
<body>
​
    <h1>Basic Table</h1>
    <table>
        <tr>
            <th>Name</th>
            <th>Occupation</th>
            <th>Years of Experience</th>
        </tr>
        <tr>
            <td>Auri Rahimzadeh</td>
            <td>Software Architect</td>
            <td>20</td>
        </tr>
        <tr>
            <td>Jenn Aikens</td>
            <td>Management</td>
            <td>15</td>
        </tr>
    </table>
​
    <br>
    <hr>
    <br>
​
    <h1>Table with Simple Border</h1>
    <table border="2">
        <tr>
            <th>Show</th>
            <th>Genre</th>
            <th>Rating</th>
        </tr>
        <tr>
            <td>The Walking Dead</td>
            <td>Horror/Drama</td>
            <td>R</td>
        </tr>
        <tr>
            <td>Breaking Bad</td>
            <td>Action/Suspense</td>
            <td>R</td>
        </tr>
    </table>
​
</body>
</html>
```

Don't forget to save your file and `alt + b` to see what your finished work looks like!

## Discussion <a id="discussion"></a>

Tables are everywhere you look in web development. You _will_ use them often. We did add one style detail to the second table using the `border` attribute, however these are not pretty tables. We will get into how to make prettier tables soon.

## Challenge <a id="challenge"></a>

Now that you've seen examples of table usage, try adding `<th>` and `<td>` tags and seeing how they interact inside of the `<table>`. Experiment with the `border` attribute some more, seeing how changing the value from 2 affects your table.

