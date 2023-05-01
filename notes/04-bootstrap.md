# Bootstrap

//NOTE - 

-bootstrap is a template for css
-css-tricks.com tonight
-justify content works horizontal align items works verticle
-learn figma tonight
-header, body, footer, are the main boxes
- flex rows go side to side to make a grid
-flex colums are each individual thing inside a row
-coloums are the amout of space we want to take up in a row
-utalizng breakpionts in bootstrap to make flex wrap easier in mobile
-rowsare horizontal, colums are space with ine rows
-it wil always go m, then rows, then colums.
-colums are essintialy saying how much space in a row you want to take up
-each colum has 12 sections
-you can have unlimited rows within the colums
-cdn from bootstrap and link it in html above the css link
- always start with a header, main, and a footer each one is a container
-container is differnet form container fluid by container fluid take up all space with no margin on the side. containers automatically add margin to the side
-next make rows in side the container 
-after the rows we and make colums
-colum 1 being the start of the page and colum 12 being the entre space the page with in the container 
-snippet <style> puts borders arounds whats been made
-put colums in side of the <class=row> divs.
-see your website in moble view in dev tools
-use section tags insted of div when using rows
-col-md-colums# sets a breakpoint and defers the set colum(12) to default to the selected -colum number when a medium ar smaller screen takes over
-name andimgae class image fluid will make it so an image will never get larger than the parent bx or container it is in.
-bootstrap has ots alreadu written componts that you can use like forms
-to center somthing along the x axis use justify content center
-bootstrap has predone colors
-inside of the parent element is where you use align amd d-flex
-margin spaces the elements to eachother
- mx-# adds margin to an element
-mb-# is for the bottom margin
-stick-top makes it so the nav bar stayes with page while scrolling
-text-center will take any text within the selected element and center it
-you can grab colums and work on them inside the dev tools
-margin will move the sctual colum and padding with adjust element inside of colum
-whith bootstrap p means padding x is horizontal y is vertical
-rounded will make a pic not have harsh corners you put this inside the image tag
- you do bootstrap callouts in side the class name
-PADDING CREATS SPACE INSIDE ON CONTAINER
-px puts padding on both sides, py puts padding on top and bottom, p puts padding all around.
-fw- for font weight
- you can put text-center and text-color and the div where the button sits(its parent element).
-bootstrap btn- for button options
- -md padding makes it so it will add padding when in mobile view
- to add icons search mdi icons and get the cdn for link ref. the use th i tag for icon and then class mdi+name of icon
-fs-# changes font size or icon size
-order inside the class name will mess the order of elements  



//NOTE - 


//NOTE - 

figma 
you can find plugins by right clicking and find more plugins
learn more about how to use figma plugins better
unsplash will take the entire image and fill the whole alotted space
you can adjust transpentacy inside the color option
at the color option you set a border by clicking color to outside
when you add text you need to create the text box
you can add test decor in the test option
drop shadow can be added in the effect section
use text box to fill the entires spce of a box and use the test options
you can crop an image in the image drop filtters
when exporting SVG is the way to go
use prototyping to set up how you want a page to react to buttons
to exit prototype view earase proto from the url in tab

//NOTE - 
//NOTE - 
use section! to use notes  and break up your html
page layout bare is 
body
header
header
main
main
footer
footer
body
stubs also are good not takers
code to mobile view first
col-md-# will set the screen to move for mobile
rows break up the page horizontally
colums run prependicular
in html everything runs vertical by default uless you use colums and rows to designate a space om the page
using an asset file is a good place to store images
after you stop images in assets you can call on them in the cod by using assets.imgID f d
best pratice for using figma is going from top to bottom
in css is where you want to make your color pallette
you can copy and paste your pallet color from figma.
put colors in the row or the colum class
use P to add padding padding works from 1-5
you can click use image an in figma by clicking view with unsplash and copy image address
in css you can call on you image class and make changes like vh and background position
using justify content in side of called upon section with move inside the row
use css glassbox generaton
you can copy and paste the glass card into you assets folder to call on it easier
puting thing inside a dive make so you can move individual from the parent element
google fonts are a great way to import fonts into your project
clink the font you want the click specimen button the left hand side to pick boldness and othe options
then copy the css link and paste in css the you can call and use that font in side html
p tags render the text smaller while h tags with make them more bold and present depending on what the text needs to represent
align-items helps move up and down and justify-items move side to side
using class=card will auto round edges and add boxshadow
and again with bootstrap you can type bg- to chang the color of whatever element you want
padding P is key with buttons and pics and cards and most elements
again addding a class to anything alows you to call on bootstrap snippets
targeting the image tags use the object properties ex. class{ object-fit}
you can use text-center instead of d-flex when the colomn and row have been set??
setting the parent element to position-relitive you can set the child element to position-absolute along with top left right bottom # to move an individual element inside of a perent element
to fulfill postion absolute make a css element and set it to postion absolute then set the height then go to html and call on the css elemnt with class=
use dev tools to manualely move thing to where you want them then copy and paste the hight width to your css file. then call on it with whatever the class is
 The .container class provides a responsive fixed width container. The .container-fluid class provides a full width container, spanning the entire width of the viewport.
 inside the css folder you can use @media(max width 768px){.class{background-image}} will make a chage such as the background-image when switching to mobileview
 margin-y=top and bottom margin-x=side to side


