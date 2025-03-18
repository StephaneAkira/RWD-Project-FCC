# Project Understanding

During the Project we have learned about the flexbox layout , how it works , and some few properties about them so far

to cretae a flex-container : we need to have display: flex ; inside that container

and any children of that container become flex-items
noe that flex-items can also be flex-container if given the display of flex;

the flexbox has the main and cross axis

this changes depending on the direction of the flexbox
if the direction is column or row
they exchange roles

flex-direction has the default as row, but we can change it to reo-reverse, column or column-reverse

justify-content : position flex-items on the main axis in FDR
align-items : position the flex-items on the cross axis in FDR

flex-wrap : nowrap as default , this will shrink flex-items in the row f needed in order to fit in one row

flex-wrap : wrap : will push flex-items in the next row and won't shrink them in order to fi in one row

gap : helps creating space between flex-items , it is a sorthand for row-gap and column-gap

giving space on top, bottom, left, and right of the flex-item

we've seen also
text-transform: uppercase
: this one puts the targeted text in uppercase , but i think more on this later with the upcoming projects

we've also seen
box-sizing: default as content-box
bu we need to set its value to border-box

more on this later as well , this is important for CSS reset

we've seen object-fit: cover;

This will tell the image to fill the img container
while maintaining aspect ratio,
resulting in cropping to fit.

i think the best practice is tp use it when working with images

we've also seen the ::after pseudo-selector
but i have no knowege about it now
let's look for it later

tha's it so far rearding the project
