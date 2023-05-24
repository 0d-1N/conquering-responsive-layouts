# conquering-responsive-layouts
its a responsive web design bootcamp of kevin in this repo i will write all my note and solve all challenges in this  bootcamp.


# the day 1 in the bootcamp :

1. percentages vs fixed width

totaly in the web when u create a index html without style ur website will be responsive automaticly
dont set a fixed width to a parent element use perecentage if the body take the full width and uset a percentage of 100% like body when u will shrink the element the element will be responsive without setting a media query for diffrent devices.

2. percentages on the child:
if u have a parent with a width and inside the parent are a child and u set a fixed width when u add a conntent inside the child maybe will overflow and this the relationship btw the parent and father u need to add the width of child with percent for exampple the parent has a width of 100% from the body and the child 50% the child will take the value of width from his parent 


3. Why it's a good idea to avoid heights:
 if u set a fixed height and u shrink the content it will be has an overflow u can just add more padding to create more background in ur layout 
 
 4. responsive typography:  
 using custom properties for example setting font size for larg and meduim and small in the root element and change it when we usse media query
 
-using vw port unit gas a n issue when zome it u can add a function call it clamp to set min and max font size

-clamp : a middlle value a range of values between a defined minimum bound and a maximum bound the function takes three parameters:a minimum value , a preferred value , and a maximum allowd value 

5. best generalisation for the right css units :
font-size : rem because its adapt for user perferences system if use px u locked it when u work with rem we use base 60 u will always need to calculate it before u declare a certain font-size if u want to work with base 10 u would add in html root element font - size element :62.5% and the body for example font-size:2.1rem its 21 px

width : the good unit to use is percentage because it will be responsive and ch ist a unit for width of char 

height : if u need a height u would chose rem and percentage and viewport unit but be careful in mobile device and work with min-height 

padding and margin : u can use em and rem it depend u want the padding or margin to be consistent despite the element that you're setting it on or if u want it to adjust based on that element's font size.

6. adding a max width :
when we setting a fixed width on ana element tends to be a bad idea , instead we can use percentages, which make our lives easier the only issue with this is at large screens,things can get too big thankfully,we have max width that setting the maximum width when u up ur layout the max-width will fix ur container growing.

7. vmin and vmax :
vmin its will tak the small viewport either width or height for example if 500 * 700 the dimensions of the viewport it will take 500 because its small so the viewport 5vw

vmax will take the large viewport etther width or height .


# the day 2 in the bootcamp :
 
1. max width :
the prblem of seeting 100% in max width not the width :
This might be a useful way to think about it: if the element would render wider than what max-width says it can be, max-width wins.
Scenarios:
Parent is 1000px wide
Width says element should be 600px wide. That doesn’t break the max-width rule, so 600px it is!
Width says element should be 1000px wide. That breaks max-width rule, so forces element down to 600px.
Parent is 320px wide
Width says element should be 600px wide. That breaks the max-width rule which says element can only be at most 320px wide, so 320px it is!
Width says element should be 320px wide. That doesn’t break the max-width rule, so 320px it is!
Whether the parent element is wider or narrower, these different rulesets end up agreeing with each other. (Although there is a difference when they are flex items.)

2. BEM : 
standads for block, element , modifier . it is a methodology and naming convention used web development to create modular and reusable ocmponents in css and html.BEM provides a systematic way to structure and organize code,making it easier to undestand maintain, and collaborate on large scale-project :

 . Block : astand alone componenet taht represents a high-level element on a webpage it is a reusable entity that can be used in diffrent contexts blocks are typicaly named with a descriptive calss name the reflects their purpose
 
 for example : header , container , menu , checkbox , input 
 
 Element : a part of a block that has no standalone meaning and semantically tied to its block :
 for expamles menu item , list item , checkbox caption , header title.
 
 Modifier a flag on a block or element use them to change appearance or behavior fo example:
         'disabled', 'highlighted','checked','fixed','size big','color yellow'.

3. flex box :
flex box is one dimensional layout method for arranging items in rows or columns , this css feature allow you to create  flexible and responsive designs by arranging elements along a single axis either horizontally or vertically.flexbox provides properties and values that control the sizing,positioning and alignment of flex items within a flex container

the crosss axis in the flex : the cross axis is the perpendicular direction to the main axis within flex container it represents the secondary axis along which flex items are aligned and distributed for example in the main axis is set to row the cross axis would run vertically,and if the main axis is set to a column, the cross axis would run horizontally.properties like "align-items" and "align-self" are used to control the postioning of flex items along this crosss axis.
. when u write the flex property u get a layout with equal size and equal height

4. flex flow :
abriviation of two properties flex direction and flex wrap
5. align content :
work like justify content but u need multiple content of lines .
6. flex shrink :
the flex-shrink its a css property sets the flex shrink factor of a flex item.if the size of all flex items is larger than the flex container , items to fit according to flex-shrink
7. flex-grow
the flex-grow its a css property sts the flex grow factor , which specifies how much of the flex coontainers remaining space should be assigned to the flex items.
8. flex basis :
how much room does this want to be taking if has the avaliable space .

9. the short hand :
flex : flex grow flex-shrink flex basis.

10. media query :
Media query is a CSS technique introduced in CSS3. It uses the @media rule to include a block of CSS properties only if a certain condition is true.

11. At-rules:
are CSS statements that instruct CSS how to behave. They begin with an at sign, '@' (U+0040 COMMERCIAL AT), followed by an identifier and includes everything up to the next semicolon, ';' , or the next CSS block, whichever comes first
