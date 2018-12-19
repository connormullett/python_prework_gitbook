# Forms

In this module we will do the following:

1. Discuss the need for the form, label, and input tags.
2. Create a basic form.
3. Discuss fieldset and consolidating all items in a form together.
4. Discuss legend tag for creating nice looking heading in border.
5. Recreate form with radio buttons and checkboxes.

## File Location <a id="file-location"></a>

For this module, you should be working in the following location:

```text

  Python_Projects
        └── prework
            └── HTMLPrework
                09-forms.html <---You should be here.
```

## Description <a id="description"></a>

It goes without saying, forms are everywhere on the web. From signing in to an application to ordering something on Amazon, we've all used forms. At some point as a new developer, you will work with forms.

## Sample Code <a id="sample-code"></a>

Add the following sample code to your file:

```text
<!DOCTYPE html>
<html>
<head>
    <title>Forms</title>
</head>
<body>
​
<h1>Forms</h1>
​
    <h2>Basic Form with input field</h2>
    <div class="form-one">
        <form>
            <p><label>Customer Name: <input></label></p>
            <p><label>Street Address: <input></label></p>
            <p><label>City: <input></label></p>
            <p><label>Area Code: <input></label></p>
            <p><label>Telephone: <input></label></p>
        </form>    
    </div> 
​
<br />
​
    <form>
        <fieldset>
            <legend> Customer Information </legend>
            <p><label>Customer name: <input></label></p>
             <p><label>Telephone: <input type=tel></label></p>
             <p><label>E-mail address: <input type=email></label></p>
        </fieldset>
    </form>
<br />
​
​
    <form>
        <fieldset>
              <legend>Biggest Burritos in the World!</legend>
            <!-- correct to look like this instead plz --><p><input type="radio" name="size" id="size1" /><label for="size1"> Humongous </label></p>
            <p><label> <input type="radio" name=size> Double-Humongous </label></p>
            <p><label> <input type="radio" name=size> Triple-Humongous </label></p>
            <p><label> <input type="radio" name=size> Just A Small, Please </label></p>
        </fieldset>
    </form>
<br/>
​
    <form>
        <fieldset>
            <legend>Fixins</legend>
            <p><label> <input type=checkbox> Sauteed Onions </label></p>
            <p><label> <input type=checkbox> Guacamole</label></p>
            <p><label> <input type=checkbox> Queso </label></p>
            <p><label> <input type=checkbox> Lettuce </label></p>
            <p><label> <input type=checkbox> Refried Beans </label></p>
            <p><label> <input type=checkbox> Rice </label></p>
        </fieldset>
    </form>
<br>
​
    <form>
        <fieldset>
            <p><label>Preferred delivery time: <input type=time min="11:00" max="21:00" step="900"></label></p>
            <p><label>Delivery instructions: <textarea></textarea></label></p>
            <p><button>Submit order</button></p>
        </fieldset>
    </form>    
</body>
</html>
​
<hr />
```

## Discussion <a id="discussion"></a>

We're starting to build on the foundation we've established, and you can probably see many of the subjects we've discussed starting to come together. In this file, we use `h1`, `h2`, `p`, `div` and, from the last lesson, `input`. We've started to describe our elements with a little more detail as well, using `attributes` on the input fields specifying the `type` that we want rendered. The result is that we're able to clearly state that we want a text box here, a checkbox there, and radio boxes in all the other places. With a solid grasp on these concepts, we're able to package elements inside of a `<form>` to describe a coherent collection of elements. `<fieldset>` empowers us to group related elements even more tightly inside a form, and also gives us access to the `<legend>` tag, which is what defines a caption for the `<fieldset>` element. Finally, the `<textarea>` tag provides a multi-line text input field. It's possible to specify the number of rows and columns within a given `<textarea>`. However, as you can see from our example, it's not necessary.

## Challenge <a id="challenge"></a>

Try experimenting with the different elements we've just learned about and incorporating previous lessons into your efforts. Test adding `attributes` like `rows` to your `<textarea>` and see how that changes what's displayed.

## Extra Reading <a id="extra-reading"></a>

​[Great resource!](https://www.w3.org/TR/html401/interact/forms.html)​

