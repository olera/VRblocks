# VRblocks or VRbilliards

A-Frame is a free web framework for building virtual reality experiences. VR content can be viewed on HTC Vive, Oculus Rift, Google Daydream, and Gear VR headsets. Even desktop and laptop PCs can display A-Frame VR content including everything from complex 3D animated objects to 360-degree panoramas.

In order to explore the space on a desktop, the user will touch and drag or click and drag to change the orientation. 

<h2>How To Use</h2>
You can use this VR space to practice moving six spheres around the grid. This will help you learn how to quickly alter the position of primitives with A-Frame. You can also play with a friend to move spheres to a claimed target, similar to calling a pocket before hitting the 8-ball in pool. Move the spheres relative to the planets, cube, and cylinders. Please fork before playing.

<h2>Credits</h2>

![cube, sphere, cylinder in VR](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTG8qzi-brMuccrS1gVPh3ecTMwuGVpJ1FEcmT2GBrIRCfj9OiJcA)

Source code for this project came from https://aframe.io/examples/ and from Mozilla.

![planetary tutotial}](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXEegtx2Gbp3qOlWGKvh-XgsYH8HNSt8MihmYU3VBBptpaAs3F)

The Mozilla tutorial on A-Frame teaches you how to create a VR version of the planets surrounding the sun. The code is available here: https://glitch.com/culture/an-intro-to-webvr/
A summary of common A-Frame attributes and tips from the tutorial follows.

<h2> A-Frame Elements </h2>

These elements are called primitives, which allow you to conveniently add entities to your space. They are similar to prefabs in Unity.

a-sky: used to alter the background with a color or 360 image
a-box: a cube. Input the color= and width= and you have generated a cube. 

Instead of using the primitive a-box, you could write the equivalent entity-component form. 

`html <a-entity geometry="primitive: box; width: 3" material="color: red"></a-entity>
`

<h2> A-Frame Tag Attributes </h2>

position: which is in the format of X, Y, Z- the 3 dimensions of space. Increasing Y for example moves up, decreasing moves down. In order to move horizontally, use positive and negative integers for X. This is the tag you will alter the most while playing the game. 
  
radius: determines how big the sphere (or planet) is.

id: a good way to let you know what the sphere is supposed to be, such as Jupiter or Mars. It can be used to reference the sphere in more advanced A-Frame scenes.

If we want two spheres together, we would wrap them in a tag called a-entity. 

# Example
In order to create ringed planets, create rings with a primitive shape called a "torus". Keep rings and planets in relative position with the a-entity tag.

A-Frame Documentation: https://aframe.io/docs/0.9.0/introduction/html-and-primitives.html
More about position: https://github.com/aframevr/aframe/blob/master/docs/components/position.md
  
 
