# Everything that is going to the head element at he moment

<meta charset="UTF-8" />
    <meta name="description" content="Quiz App" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Learn Accessibiliy by Building a Quiz</title>
    <link rel="stylesheet" href="./CSS/styles.css" />
we've added the : <meta name="description" content="Quiz App" />

- Navigation is a core part of accessibility, and screen readers rely on you
  to provide the structure of your page.
  This is accomplished with semantic HTML elements.

- Add a header and a main element to your page.

The header element will be used to introduce the page,
as well as provide a navigation menu.

The main element will contain the core content of your page.

- min() and max(): on font-size and width , i guess on some other tings as well

- As this is a quiz, you will need a form for users to submit answers.
  You can semantically separate the content within the form using
  section elements.

- To increase the page accessibility, the role attribute can be used to
  indicate the purpose behind
  an element on the page to assistive technologies.
  The role attribute is a part of the Web Accessibility Initiative (WAI),
  and accepts preset values.

- Give each of the section elements the region role.
- Every region role requires a label, which helps screen reader users
  understand the purpose of the region.
  One method for adding a label is to add a heading element inside the region
  and then reference
  it with the aria-labelledby attribute.

- nest one h2 element with an id matching the corresponding
  aria-labelledby attribute. Give each h2 suitable text content.

- To be able to navigate within the page, give each anchor element
  an href corresponding to the id of the h2 elements.

- It is important to link each input to the corresponding label element.
  This provides assistive technology users with a visual reference to the
  input.

This is done by giving the label a for attribute,
which contains the id of the input.

- Keeping in mind best-practices for form inputs, give each input an
  appropriate type and name attribute.
  Then, give the first input a placeholder attribute.

- The question numbers are not descriptive enough.
  This is especially true for visually impaired users.
  One way to get around such an issue,
  without having to add visible text to the element,
  is to add text only a screen reader can read.

Nest a span element with a class of sr-only after the number
in each of the h3 elements.

- The .sr-only text is still visible. There is a common pattern
  to visually hide text for only screen readers to read.

This pattern is to set the following CSS properties:

Example Code
position: absolute;
width: 1px;
height: 1px;
overflow: hidden;
clip: rect(0, 0, 0, 0);
clip-path: inset(50%);
white-space: nowrap;
Use the above to define the .sr-only CSS rule.

- If you click on the radio inputs, you might notice both inputs
  within the same true/false fieldset can be selected at the same time.

Group the relevant inputs together such that only one input from a pair
can be selected at a time. A/ Hint we use the name attribute
to accomplish that
by giving the concerned group of radio the same name attribute

To prevent unnecessary repetition,
target the before pseudo-element of the h3 element,
and give it a content property of "Question #"

- Link the first label element to the select element,
  and give the select element a name attribute.

A/ Hint: for attribute on label same as the id of the select element

- Two final semantic HTML elements for this project are the footer
  and address elements. The footer element is a container for a collection of content that is related to the
  page, and the address element is a container for contact information
  for the author of the page.

After the main element, add one footer element,
and nest one address element within it.

- Clicking on the navigation links should jump the viewport to
  the relevant section. However, this jumping can be disorienting for some users.

Select all elements, and set the scroll-behavior to smooth

it has been great and usefull explanation overall

i hope for more breakdowns next-time
