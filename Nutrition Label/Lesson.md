We used a lot of utility classes that are important for positioning element or creating a divider with different size for different pusposes

like :

.bold ; .right ; .divider ; .medium ; .large ; .small-text ; .indent etc...

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

- following the structure of the project is self-explanatory

# Typography In depth

Typography is the way that text is arranged and presented

we will work with Text and Fonts

- Example With Text
  p{
  text-decoration: underline
  text-decoration: line-through
  text-decoration: none (this is he default for text)
  text-transform: capitalise
  text-transform: lowercase
  text-transform: uppercase

  text-align:left(this is the default)
  text-align: justify(use for Magazine)
  text-align: right
  text-align: center
  text-indent: 1em (provide indentation) it indents the first line

  line-height: 1.2(is the default) 1.5 is better and looks cleaner and more readable

  letter-spacing: ; (increase the space between the letters of the word), the Default is fine unless you want smething Specific

  word-spacing: ; just like letter-spacing , the default is fine unless...

}

example with Font

p{
font-weight:noraml(is the default)
font-style: italic, oblic (a strong italic)

}

body{
font-family:serif, sans-serif, monosapce , cursive, fantasy
(those are generic families , mostyused as fallbacks)
if the font family has a space in it we need quotes:"", else we dnon't need quotes
}

fonts.google.com : we can use it to get fonts

# How to Set fonts in our Project

a link we can put in the head element of the HTML

copy the Link
then pase it inside the head of your code
before the link of the stylesheet, your CSS

in the CSS
use
fon-family: then put whatever U took from fontsgoogle.com

it lags the loading of the page
if you stack a lot of fonts
