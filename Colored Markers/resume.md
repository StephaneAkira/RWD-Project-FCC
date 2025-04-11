# What we will Learn

Selecting the correct colors for your webpage can greatly improve the aesthetic appeal to your readers.

In this course, you'll build a set of colored markers. You'll learn different ways to set color values and how to pair colors with each other.

# HTML

we learnt about the div element which are specifically used as containers

# CSS

It's better practice to choose one color as the dominant color,
and use its complementary color as an accent to bring attention
to certain content on the page.

To center your marker on the page,
set its margin property to auto.

To give the markers different colors, you will need to add a
unique class to each one.
Multiple classes can be added to an element by listing them in the
class attribute and separating them with a space.
For example, the following adds both the animal and dog classes
to a div element.

Example Code

<div class="animal dog">

NB: If you add multiple classes to an HTML element,
the styles of the first classes you list may be overridden by later classes.

we talked colors :
There are two main color models: the additive RGB (red, green, blue)
model used in electronic devices,
and the subtractive CMYK (cyan, magenta, yellow, black)
model used in print.

# rgb():

Example Code
rgb(red, green, blue);
Each red, green, and blue value is a number from 0 to 255.
0 means that there's 0% of that color, and is black.
255 means that there's 100% of that color.

In the additive RGB color model, primary colors are colors that,
when combined,
create pure white. But for this to happen,
each color needs to be at its highest intensity.

background-color: rgb(255, 255, 255);
this is white

Secondary colors are the colors you get when you combine primary colors.
You might have noticed some secondary colors in the last step as you
changed the red, green, and blue values

To create the first secondary color, yellow,
update the rgb function in the .one CSS rule to combine
pure red and pure green.

To create the next secondary color, cyan,
update the rgb function in the .two CSS rule to combine
pure green and pure blue.

Now that you're familiar with secondary colors, you'll learn how
to create tertiary colors.
Tertiary colors are created by combining a primary
with a nearby secondary color.

To create the tertiary color orange,
update the rgb function in the .one CSS rule so
that red is at the max value, and set green to 127.

Notice that, to create orange,
you had to increase the intensity of red and decrease the intensity of
the green rgb values.
This is because orange is the combination of red and yellow.

To create the tertiary color spring green,
combine cyan with green. Update the rgb function in the .two CSS rule so
that green is at the max value,
and set blue to 127.

And to create the tertiary color violet,
combine magenta with blue. Update the rgb function in the .three CSS rule
so that blue is at the max value,
and set red to 127.

There are three more tertiary colors: chartreuse green (green + yellow),
azure (blue + cyan),
and rose (red + magenta).

To create chartreuse green, update the rgb function in the .one CSS rule
so that red is at 127,
and set green to the max value.

For azure,
update the rgb function in the .two CSS rule
so that green is at 127 and blue is at the max value.

And for rose,
which is sometimes called bright pink, update the rgb function
in the .three CSS rule so that blue is at 127 and
red is at the max value.

Now that you've gone through all the primary, secondary, and tertiary colors on a color wheel,
it'll be easier to understand other color theory concepts and how they
impact design.

A color wheel is a circle where similar colors, or hues,
are near each other, and different ones are further apart.
For example, pure red is between the hues rose and orange.

Two colors that are opposite from each other on the color wheel are called
complementary colors.
If two complementary colors are combined,
they produce gray. But when they are placed side-by-side,
these colors produce strong visual contrast and appear brighter.

# hsl():

The HSL color model, or hue, saturation, and lightness,
is another way to represent colors.

The CSS hsl function accepts 3 values: a number from 0 to 360 for hue,
a percentage from 0 to 100 for saturation,
and a percentage from 0 to 100 for lightness.

If you imagine a color wheel,
the hue red is at 0 degrees, green is at 120 degrees,
and blue is at 240 degrees.

Saturation is the intensity of a color from 0%, or gray, to 100% for pure
color.
You must add the percent sign % to the saturation and lightness values.

Lightness is how bright a color appears, from 0%, or complete black, to 100%

# #hex:

Hex color values start with a # character and take six characters
from 0-9 and A-F.
The first pair of characters represent red, the second pair represent green,
and the third pair represent blue. For example, #4B5320.

You may already be familiar with decimal, or base 10 values,
which go from 0 - 9.
Hexadecimal, or base 16 values, go from 0 - 9, then A - F:

Example Code
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F
With hex colors, 00 is 0% of that color, and FF is 100%.
So #00FF00 translates to 0% red, 100% green, and 0% blue,
and is the same as rgb(0, 255, 0).
Lower the intensity of green by setting the green value of the hex color
to 7F

# linear-gradient():

A gradient is when one color transitions into another.
The CSS linear-gradient function lets you control the direction
of the transition along a line,
and which colors are used.

One thing to remember is that the linear-gradient function actually
creates an image element,
and is usually paired with the background property
which can accept an image as a value.

Example Code
linear-gradient(gradientDirection, color1, color2, ...);

The linear-gradient function is very flexible -- here is the basic
syntax you'll use in this tutorial:

First, in the .red CSS rule, set the background property to linear-gradient(),
and pass it the value 90deg as the gradientDirection

You won't see gradient yet because the linear-gradient function needs
at least two color arguments to work.

In the same linear-gradient function,
use the rgb function to set the second color argument to pure green.

As you can see, the linear-gradient function produced a smooth red-green
gradient.
While the linear-gradient function needs a minimum of two color arguments
to work,
it can accept many color arguments.

Color-stops allow you to fine-tune where colors are placed
along the gradient line. They are a length unit like px or percentages
that follow a color in the linear-gradient function.

For example, in this red-black gradient,
the transition from red to black takes place at the 90% point along
the gradient line, so red takes up most of the available space:

Example Code
linear-gradient(90deg, red 90%, black);

If no gradientDirection argument is provided to the linear-gradient function,
it arranges colors from top to bottom, or along a 180 degree line,
by default.

# Gradients In depth Guide

we use gradient with the background property

we need at least two colors for the gradient to work

# Linear Gradient

- background: linear-gradient(teal,purple)

- we can change directions by specifying at the beginning before the colors like so:

background: linear-gradient(to bottom or 123deg, teal,purple)

- we can control the size of the colors , we call it color-stop, we can specify % after a color we have a starting and a closing % , we need both
  like so :

background: linear-gradient(teal 0% 10%,purple 40% 100%)

# Radial Gradient

it radiates outward from an origine
of a form of a circle but often elipse

background: radial-gradient(teal,purple)

- we can make he origine a circle rather than an elipse,
  by specifying circle before the colors.

  note that we can soecify color-stop just like with liner-gradient
  like so :

background: raial-gradient(circle , teal,purple)

- we can also position the origine
  by specifying the circle or whatever we want thenn at choose a postion we want that to be
  like so:

background: radial-gradient(circle at top , teal,purple)

# Conic Gradient

it's nice looking
use at least 2 colors , but use 8 for good looking points

in a conic gradient, colors rotate around some central point

- we can change the color-stop just like any other gradient, we can position them etc... just like the rest of them

# repeating gradient:

we have repeating versions of gradients, linear, conic or radial

let's see some example

let's set color-stop values with px

- background: repeating-linear-gradient(teal 50px,purple 50px 100px, teal 100px 150px)

- background: repeating-radial-gradient(teal 50px,purple 50px 100px, teal 100px 150px)

- background: repeating-conic-gradient(teal 50px,purple 50px 100px, teal 100px 150px)

# Opacity:

With the CSS opacity property, you can control how opaque or transparent
an element is.
With the value 0, or 0%, the element will be completely transparent,
and at 1.0, or 100%, the element will be completely opaque like it is
by default.

Another way to set the opacity for an element is with the alpha channel.
Similar to the opacity property,
the alpha channel controls how transparent or opaque a color is.

You've already set sleeve's opacity with a named color and the opacity
property,
but you can add an alpha channel to the other CSS color properties.

Inside the .sleeve rule, remove the opacity property and value

You're already familiar with using the rgb function to set colors.
To add an alpha channel to an rgb color, use the rgba function instead.

The rgba function works just like the rgb function,
but takes one more number from 0 to 1.0 for the alpha channel:

Example Code
rgba(redValue, greenValue, blueValue, alphaValue);
You can also use an alpha channel with hsl and hex colors.

NB:
To position two div elements on the same line,
set their display properties to inline-block.

For a border to be visible, you need to set its width and style.

The border-left shorthand property lets you to set
the left border's width, style, and color at the same time.

Here is the syntax:

Example Code
border-left: width style color;

# box-shadow:

The box-shadow property lets you apply one or more shadows around an element.
Here is basic syntax:

Example Code
box-shadow: offsetX offsetY color;

Here's how the offsetX and offsetY values work:

both offsetX and offsetY accept number values in px and other CSS units
a positive offsetX value moves the shadow right and a negative value moves it left
a positive offsetY value moves the shadow down and a negative value moves it up
if you want a value of zero (0) for any or both offsetX and offsetY, you don't need to add a unit.
Every browser understands that zero means no change.

The height and width of the shadow is determined by the height and width
of the element it's applied to.
You can also use an optional spreadRadius value to spread out the reach
of the shadow. More on that later.

Start by adding a simple shadow to the red marker.

In the .red CSS rule, add the box-shadow property
with the values 5px for offsetX, 5px for offsetY, and red for color.

As you can see, you added a simple red shadow around your marker
that's 5 pixels to the right, and 5 pixels down.

But what if you wanted to position your shadow on the opposite side?
You can do that by using negative values for offsetX and offsetY

Notice that the edges of the shadow are sharp.
This is because there is an optional blurRadius value for the box-shadow
property:

Example Code
box-shadow: offsetX offsetY blurRadius color;
If a blurRadius value isn't included, it defaults to 0 and produces
sharp edges.
The higher the value of blurRadius, the greater the blurring effect is.

But what if you wanted to expand the shadow out further?
You can do that with the optional spreadRadius value:

Example Code
box-shadow: offsetX offsetY blurRadius spreadRadius color;

# What Stood out to me

box-shadow:

# Project Structure

a h1
3 divs for each of the markers
colors , linea gradient for each markr or div
double border and a transparent class of sleeve to seal the deal
