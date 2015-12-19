---
layout: page
title: Amusement Park
list: no
=======


#OpenGL Amusement Park
This project, “An Amusement Park” uses OpenGL to draw a virtual amusement park. The park includes Ferris Wheel, Columbus Ship Ride and Roller Coaster. 

See the [YouTube video](https://www.youtube.com/watch?v=7_Z5359IEVU) for a walkthrough.

<iframe width="560" height="315" src="https://www.youtube.com/embed/7_Z5359IEVU" frameborder="0" allowfullscreen></iframe>

###Giant wheel
Giant Wheel is visualized using circular rings. Rotation effects are provided for Giant Wheel. 

###Ship Ride
Swinging action is employed for Columbus ship. 

###Roller Coaster
The Roller Coaster moves on a specified track. The tracks are created using Bezier curve functions with a set of defined control points, which are configurable. Tracks can also be placed on a separate file to enable dynamic loading of track data. 

###Skybox
The whole scene is placed inside a texture mapped cube called SkyBox. This gives a realistic sky effect. 

###Movement
The software also includes a first person movement where the viewer can move around anywhere in the scene. Mouse drag for rotation is supported.

###More Options
The mouse context menu helps the user in selecting various options. The colours of various objects can be changed. The SkyBox texture background can be changed. The user can control various camera positions like, Free Movement, On Roller Coaster, On Columbus ship and In Giant Wheel. The user will also be able to control the movement of individual objects.


Objects like cube, sphere and cylinders are used to implement 3D objects. Plain lines are used in the construction of Roller Coaster track. The normal, tangent and binormal at every point on the curve is calculated and the Roller Coaster is properly oriented along the track by rotating it about the angles made by tangent, normal and binormal with the curve.
The following options are supported:
•	Navigate in the scene. Rotate 360 degree to view.
•	Start and stop Giant Wheel rotation, Columbus swinging action and Roller Coaster movement.
•	Change colours of Giant Wheel, Columbus ship and Roller Coaster.
•	Change background of SkyBox.


##Screenshots:
![1](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/1.png)
![2](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/2.png)
![3](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/3.png)
![4](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/4.png)
![5](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/5.png)
![6](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/6.png)
