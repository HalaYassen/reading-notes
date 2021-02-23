# Transforms in CSS
it is property to control in the position of an elements. 

**The Syntax of Transform:**
syntax is including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses, the following example rotate the element (60 degree ) 
`transform: rotate(60deg)`

Transformation divided to the two settings which is :

1. two-dimensional "2D_Transforms"

Changing element on two dimensions which is `x` and `y`, x or y values to the scale property to change the size either in horizantally (x) or  vertically(y)  

* you can change using 2D Transforms:

**Rotate:**rotate value provid rotate an element from 0 to 360 degrees(which is called full circle).

**Translate:** to shift the element in any direction.

**Scale:** the scale value is to change the appeared size of an element, because the default scale value is one, any value greater than or equal to one makes an element appear in a big size! 

this example show how `transform: scale(.55)` in this example the size changed to 55% for an element to apears big than from original size!


2. three-dimensional "3D_Transforms"
changing the element in three dimensional scale x , y , z .

 here are somethings that you can change using 3D Transforms:

**Rotate:** you can rotate an element around any one of any axes you want, so we use three values, `rotate X`, `rotate Y`, `rotate Z.`

**we use:** 
* `rotate X` to rotate an element around the X axis, as in half horizontally.

* `rotate Y` to rotate an element around the Y axis, as  in half vertically. 

* `rotate Z` to rotated around completely the Z axis.


**Scale:** using scale Z (3d_tras.) transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. 

**Each of them(2-D/3-D) comes with their own individual properties and values**