---
layout: page
title: 3D Amusement Park
list: no
---

This project, “An Amusement Park” uses OpenGL to draw a virtual amusement park. The park includes Ferris Wheel, Columbus Ship Ride and Roller Coaster, all drawn using basic OpenGL primitives.

See the [YouTube video](https://www.youtube.com/watch?v=7_Z5359IEVU) for a walkthrough.

<iframe width="560" height="315" src="https://www.youtube.com/embed/7_Z5359IEVU" frameborder="0" allowfullscreen></iframe>

The primary goal of this project was to apply the different OpenGL techniques I had learnt into a project ready for demonstration. When I thought about the scene on which I should be building on, Amusement Park came to my mind as it can involve different kind of movements associated with different kind of objects. 

###Giant wheel
The Giant wheel or the Ferris wheel was the first object I attempted to recreate. As a combination of torus, disc and inflated lines formed the skeletal part of the wheel, the trolley was formed by placing multiple cubes and rotating each about their center. Next, every such trolley had to be upright with respect to the wheel, which I achieved by rotating the trolley along the angle made by it with the center of the torus. When the wheel rotates, each trolley has to be rotated by the same angle so that they all will remain upright. However, with a slight distortion that I applied using trigonometric functions, I was able to create a *swinging effect* for each trolley, which can be observed in the video.

![Trolley rotation](http://akarthik10.github.io/public/cgv/cgv_trolley_rotate.PNG)

This was the output:

![1](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/1.png)
![2](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/2.png)


###Ship Ride
The ship ride, also known as the Columbus ship was the most straightforward object to recreate. The base of ship came from a half cut elongated ellipsoid. The ship swings with respect to the point where it is attached to the stand. This swinging action was created using a trigonometric function of a specific period (time).

![3](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/3.png)
![4](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/4.png)


###Roller Coaster
The roller coaster was one of the most challenging things in this project. The challenges were to:

- Draw a predetermined track along a specified path
- Move the roller coaster car along it
- Place the camera on one of the seats in the car and follow it as it moves
- Change the car orientation according to the orientation of the track
- Continually vary speed of the car based on whether it is climbing or descending

A set of multiple Bezier curves were joined together to form a smooth, long and continuous track on which the roller coaster car could move. This also involved algorithms that smoothened a jerky transition from one Bezier curve to another. By calculating the normal, bi-normal and tangent at every position of the car, I was able to control the pitch, yaw and roll of the car to make it look realistic.

![Trolley rotation](http://akarthik10.github.io/public/cgv/cgv_normal_bi_tan.PNG)

Eventually, this is how it turned out to be:

![5](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/5.png)
![6](https://github.com/akarthik10/AmusementPark/raw/master/screenshots/6.png)

###Skybox
The realistic sky background effect is achieved using the skybox technique. In this technique, the scene is placed in a very large cube with the inner walls of the cube textured with images of sky. The box also moves with respect to the first person camera, but at a much slower rate so that a parallax effect is achieved.

![Skybox](http://akarthik10.github.io/public/cgv/cgv_skybox.PNG)

The above image shows the skybox with a containing scene.

###Other options
There are several other options including:

* First person and second person camera movement
* Mouse drag and pull support for navigation
* Configurable skybox backgrounds
* Configurable camera positions using context menu
* Configurable colors of every object

For more details, see the complete report: [3D Amusement Park - Project Report](https://drive.google.com/file/d/0B6TfmI2fgbDyYTZhRVJuLTh1NTQ/view?usp=sharing&resourcekey=0-t4EKr35Z5uEJpBQRudK6wQ)

The below diagram provides a high level overview of implementation level details

![Flowchart](http://akarthik10.github.io/public/cgv/cgv_flowchart.PNG)

