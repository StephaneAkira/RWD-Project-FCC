We have just completed he project

during the project we have learnt a lot about

CSS Positioning
a little bit of CSS transform with the rotate property that uses deg

# CSS Positioning

- We have 5 position values in total
- Static, Absolute, Fixed, Sticky and Relative

# Absolute:

an element with the position:absolute
we will see the effect immediately

it is removed from the HTML document
other elements will behave as if it's not there, it's not existing anymore in the document

it can be moved using top, bottom, left and right

top : 0; : will be at the top of the document
left: 0; : will place it at the left of the document
same for the other stuff

a negatif number will put the element outside of the document

that may create an horizontal scrolling
we can use overflow-x: hidden; on the body to fix things up

Note that position: absolute;
is relative to the entire page

if we want it to be relative to something else like it's parent container , we need to give the parent a position: relative;

so the child with the position absolute can be relative to its parent container

if the child with position absolute doesn't find a parent or any other container with a position relative the it revert to the HTML as the parent

now since absolute is not in the document it will be overlapping other element
to set it under an element we can give it a z-index of -1;

# Static

an element with position:static;

Static don't have access to the
top,left,right or bottom or the z-index

# Relative

an element with the position: relative;

no effect is immediate

but relative has the access to
left,right,top and bottom even the z-index

element of the position: relative;
stay in the normal flow of the document

so top: 100px will put the element 100px away from the top of the container

# Fixed

an element with the position of fixed
is removed from the document flow just like absolute and the effect is immediate just like with absolute

it has access to everything

but the position of the element with the position : fixed ;
stays at the same place when scrolling

and it is always relative to the HTML or the entire page no matter what

we can use it for headers or footers

giving it a width of 100%
top : 0
left: 0
replacing top with bottom : 0;
will actually make it a footer
z-index:1;

# Sticky

sticky is quite tricky
an element with the position of sticky
doesn't have an immediate effect

but has access of everything
and works similarly to fixed

if we give top:0px;

when scrolling , the element will stick once it reaches the end of the container, but i'll need more explanation for this part alone

and some extended version of border radius and note that border-radius helps in shaping things into a circular shape

- we also saw z-index for the first time , i'll need tutorials about it as well
- A/ z-index of -1 : will set the element above another element if we're overlaping

z-index of 1 just do the opposite of -1;
