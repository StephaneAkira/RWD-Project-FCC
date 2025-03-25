We used a lot of utility classes that are important for posiioning element or creating a divider with different size for different pusposes

like :

.bold ; .right ; .divider ; .medium ; .large ; .small-text ; etc...

# CSS side:

- The letter-spacing property can be used to adjust the space between
  each character of text in an element.

- Nutrition labels have a lot of bold text to draw attention to
  important information.
  Rather than targeting each element that needs to be bold,
  it is more efficient to use a class to apply
  the bold styling to every element.

- The rem unit stands for root em,
  and is relative to the font size of the html element.

  - alignment is also important
    Notice how the text 8g appears centered in the preview.
    Nest the span element containing the text Total Fat along with the text 8g,
    in an additional span element for alignment.

        -

    Add no-divider to the class for these two elements.

The :not pseudo-selector can be used to select all elements
that do not match the given CSS rule.

Example Code
div:not(#example) {
color: red;
}
The above selects all div elements without an id of example.

-following the structure of the project is self-explanatory
