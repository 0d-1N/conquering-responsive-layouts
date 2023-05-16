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
