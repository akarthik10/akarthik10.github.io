---
layout: page
title: 3D Amusement Park
list: no
---

This project, “An Amusement Park” uses OpenGL to draw a virtual amusement park. The park includes Ferris Wheel, Columbus Ship Ride and Roller Coaster, all drawn using basic OpenGL primitives.

See the [YouTube video](https://www.youtube.com/watch?v=7_Z5359IEVU) for a walkthrough.

<iframe width="560" height="315" src="https://www.youtube.com/embed/7_Z5359IEVU" frameborder="0" allowfullscreen></iframe>

The primary goal of this project was to apply the different OpenGL techniques I had learnt into a demonstration ready project. When I thought about the scene on which I should be building on, Amusement Park came to my mind as it can involve different kind of movements associated with different kind of objects. 

###Giant wheel
The Giant wheel or the Ferris wheel was the first object I attempted to recreate. As a combination of torus, disc and inflated lines formed the skeletal part of the wheel, the trolley was formed by placing multiple cubes and rotating each about their center. Next, every such trolley had to be upright with respect to the wheel, which I achieved by rotating the trolley along the angle made by it with the center of the disc. When the wheel rotates, each trolley has to be rotated by the same angle so that they all will remain upright. However, with a slight distortion that I applied using trigonometric functions, I was able to create a *swinging effect* for each trolley, which can be observed in the video.


![1](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/1.png)
![2](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/2.png)

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

![3](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/3.png)
![4](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/4.png)
![5](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/5.png)
![6](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/6.png)


The complete project report can be viewed below.

<iframe src="https://drive.google.com/file/d/0B6TfmI2fgbDyYTZhRVJuLTh1NTQ/preview" width="640" height="480"></iframe>


