#

building a signup page. You'll learn how to control what types of data people can type into your form, and some new CSS tools for styling your page.

# HTML

# we talked about the form element

The method attribute specifies how to send form-data to the URL
specified in the action attribute.
The form-data can be sent via a GET request as URL parameters
(with method="get") or
via a POST request as data in the request body (with method="post").

As the form will have three distinct sections,
add three fieldset elements within the form element.

we can separate sections or parts inside the form with the fieldset element

input and label need to be linked with the same value for rhe for attribute in the label and the id of the input element

The first input element with a type of submit is
automatically set to submit its nearest parent form element.

To handle the form submission, after the last fieldset element add an
input element with the type attribute
set to submit and the value attribute set to Submit.

To make the form more interactive,
add the required attribute to the input elements in the first fieldset.

Add custom validation to the password input element,
by adding a minlength attribute with a value of 8.
Doing so prevents inputs of less than 8 characters being submitted.

With type="password" you can use the pattern attribute to define a
regular expression
that the password must match to be considered valid.

Add a pattern attribute to the password input element to require
the input match: [a-z0-5]{8,}

The above is a regular expression which matches eight or
more lowercase letters or the digits 0 to 5.
Then, remove the minlength attribute, and try it out.

You only want one radio input to be selectable at a time. However,
the form does not know the radio inputs are related.

To relate the radio inputs, give them the same name attribute with a value
of account-type.
Now, it is not possible to select both radio inputs at the same time.

Follow accessibility best practices by linking the input elements and
the label elements in the second fieldset.

Moving on to the final fieldset.
What if you wanted to allow a user to upload a profile picture?

Well, the input type file allows just that.
Add a label with the text Upload a profile picture:
, and nest an input accepting a file upload.

Add another label after the first, with the text Input your age (years): .
Then, nest an input with the type of number.

Next, add a min attribute to the input with a value of 13 because users
under the age of 13 should not register.
Also, users probably will not be over the age of 120;
add a max attribute with a value of 120.

Now, if someone tries to submit the form with values outside of the range,
a warning will appear, and the form will not submit. Give it a try.

Adding a dropdown to the form is easy with the select element.
The select element is a container for a group of option elements,
and the option element acts as a label for each dropdown option.
Both elements require closing tags.

Submitting the form with an option selected would not send a useful
value to the server.
As such, each option needs to be given a value attribute.
Without which, the text content of the option will be submitted
to the server.

Give the first option a value of "",
and the subsequent option elements value attributes from 1 to 4.

The textarea element acts like an input element of type text,
but comes with the added benefit of being able to receive multi-line text,
and an initial number of text rows and columns.

The textarea appears too small.
To give it an initial size, you can add the rows and cols attributes.

Add an initial size of 3 rows and 30 columns.

To give Campers an idea of what to put in their bio,
the placeholder attribute is used.
The placeholder accepts a text value, which is displayed until the
user starts typing.

Give the textarea a placeholder of I like coding on the beach...

The HTML for the registration form is finished.
Now, you can spruce it up a bit.

Start by adding Tahoma as the font with a font size of 16px in the
body selector.

For the second fieldset,
you want the input and label text to appear on the same line.

Start,
by giving the input elements in the second fieldset a class of inline

# CSS

- The vh unit stands for viewport height, and is equal to 1% of the height of the viewport.
  This makes it relative to the viewport height.

- Now, get rid of the horizontal scroll-bar,
  by setting the body default margin added by some browsers to 0.

- The rem unit stands for root em,
  and is relative to the font size of the html element.

- As label elements are inline by default,
  they are all displayed side by side on the same line,
  making their text hard to read. To make them appear on separate lines,
  add display: block to the label element,
  and add a margin of 0.5rem 0, to separate them from each other.

- The border of the last fieldset element looks a little out of place.
  You can select the last element of a specific type using the
  last-of-type CSS pseudo-class, like this:

Example Code
p:last-of-type { }
That will select the last p element.

- It would be nicer to have the label text appear above the form elements.

Select all input, textarea, and select elements,
and make them take up the full width of their parent elements.

Also, add 10px of margin to the top of the selected elements.
Set the other margins to 0.

Select only the .inline elements, and give them width of unset.
This will remove the earlier rule which set all the input elements
to width: 100%.

- If you look close enough, you will notice the .inline elements are too
  high on the line.

To combat this, set the vertical-align property to middle.

- You want the select element to remain with a white background,
  but now it is not getting the same min-height as the input and
  textarea elements.

Move the min-height property and value so that all three element
types have the same min-height value,
and the select element still has a white background.

- To style the submit button, you can use an attribute selector,
  which selects an element based on the given attribute value.
  Here is an example:

Example Code
input[name="password"]

The above selects input elements with a name attribute value of password.

- To make the submit button appear more distinct,
  give it a background-color of #3b3b4f, and a border-color of white

Lastly, for the submit button, you want to separate it from the fieldset
above,
and adjust its width to never be below 300px.

Change the margin property to include 1em on the top and bottom,
while leaving the right and left margins set to auto.
Then set the width as described above.

-

# What stood out to me

# Project Structure
