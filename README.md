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
