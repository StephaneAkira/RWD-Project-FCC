We have built a Piano using
a little bit of everything we have learnt so far
we even have used the float property

we used overflow hidden , on the original class so when use the media querry the elements won't overlap

we used @media

but i'll need more explanation or tutorial to fully grasp it

# Media Queries

- allow us to target specific viewport sizes and apply styles on them

- syntax:

  - by default it targets all , and most of the time we want to target all media types : screen , speech, print etc...

  - inside the parentheses we can add the breakpoints

  - let's explain (max-with) and (min-width)

  - (max-width : 500px):
    max-width:500px just means that
    it will target screens below the breakpoint of 500px

  - (min-width:500px):
    min-width:500px just means that it will target screens above the breakpoint of 500px

    Note:

    - if you want to design your app or website Desktop first

    "use max-width": to make the site responsive on smaller viewport

    - if you want to design your app or website Mobile First

    "use min-width": to make the site responsive on larger viewport

- It's Best Practice to use pre-defined Breakpoints instead of creating a @media everytime the layout breaks

* XS : Extra Small screen
  @media (min-width: 475px){}

* SM : small screen
  @media (min-width: 640px){}

* MD : Medium Screen
  @media (min-width: 768px){}

* LG : Large Screen
  @media (min-width: 1024px){}

* XL : Extra Large Screen
  @media (min-width: 1280px){}

* XXL : Extra Extra Large Screen
  @media (min-width: 1536px){}

  @media () {
  inside here we can select whatever we want : ids, classes etc.. and style them according to each breakpoint
  }

  # Side Note:

  it's good practice while working on a project to have a .container (utility class) that will figure in every section of the project
  and also avoid using shorthand for properties code them individually

  for mobile first
  .container{
  width : 100%
  marin-left: auto
  marin-right: auto
  padding-left: 0.5rem
  padding-right: 0.5rem
  }

  inside each media Queries
  @media
  .container{
  max-width: of whatever the min-width is on the @media declaration

  this smooths the layout breakpoint , so everytime the viewport touches the border of the sections it wil break and it also helps with a really good alignment
  }

  for Deskop First

  .container{
  width : 1536px
  marin-left: auto
  marin-right: auto
  padding-left: 0.5rem
  padding-right: 0.5rem
  }

  inside each media Queries
  @media

  .container{
  a picture wil be provided
  }

  and avoid the popular
  width of 90% and margin of 0 auto

Pseudo selector ::before and ::after
more on this later
