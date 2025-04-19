The Project is Over

During this Project we went over a lot of stuff , some old, some new , but the headliner was the use of CSS grid to shape out the layout

aight let's start from the begining
but before that
nte that we can create columns without the Grid layout
just with width:column then give it a rem or px % or whatever that works

note:
text-align: justify; works well with a magazine type of project

# Layout

- we have a main container that has everything inside it

- we have have 3 section in this projects

- we have used the CSS grid to Layout this Magazine Project

- to make a container to be a grid parent just
  Display: grid

- inside the parent we have a lot of properties that can go in

# CSS GRID

note: grid helps use to layout the page and also has access to overlapping elements

- first of all we need to make main our grid parent , because everything will go through it

- regarding properties we can use

- grid-template-columns: this helps to create columns for the container
  eg.:
  grid-template-columns: 1fr 2fr

will create two columns in that container the first with 1fr and the second with 2fr , ( fr: fraction)

we also have used minmax function

- we can use grid-template-columns: repeat( 3, 1fr) : for example this will create 3 columns of 1 fr for each column

- we can also use column-gap: to create space between columns

- we can also use row-gap to create space between rows

- or use a shorthand just like with flexboxes , it takes 2 values,
  row-gap is for the first value, and column-gap is for the second value
  if only one value is given then it's for both

- we can also use grid-template-rows:
  works just like grid-template-columns:
  but for rows
  eg.:
  grid-template-rows: 1fr 2fr

will create two rows in that container the first with 1fr and the second with 2fr , ( fr: fraction)

- grid-auto-flow: If you wanted to add more social icons, but keep them on the same row, you would need to update grid-template-columns to create additional columns. As an alternative, you can use the grid-auto-flow property.

This property takes either row or column as the first value, with an optional second value of dense. grid-auto-flow uses an auto-placement algorithm to adjust the grid layout. Setting it to column will tell the algorithm to create new columns for content as needed. The dense value allows the algorithm to backtrack and fill holes in the grid with smaller items, which can result in items appearing out of order.
For your .social-icons selector, set the grid-auto-flow property to column.

- grid-auto-columns: Now the auto-placement algorithm will kick in when you add a new icon element. However, the algorithm defaults the new column width to be auto, which will not match your current columns.

You can override this with the grid-auto-columns property. Give the .social-icons selector a grid-auto-columns property set to 1fr.

# for the Items of the grid there are a lot of propperties we can use as well

s

- grid-column: One option is the grid-column property, which is shorthand for grid-column-start and grid-column-end. The grid-column property tells the grid item which grid line to start and end at.
-

# Minmax(): more on this later
