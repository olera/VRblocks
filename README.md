# VRblocks

A-Frame is a free web framework for building virtual reality experiences. VR content can be viewed on HTC Vive, Oculus Rift, Google Daydream, and Gear VR headsets, 
as well as desktop and laptop PCs, including everything from complex 3D animated objects to 360-degree panoramas.

In order to explore the space on a desktop, click and drag to change the orientation. 

Source code for this project came from https://aframe.io/examples/ 

Mozilla also offers a tutorial on A-Frame, available here: https://glitch.com/culture/an-intro-to-webvr/
A summary of the Mozilla tutorial follows.

<script src="https://aframe.io/releases/0.8.2/aframe.min.js"></script>
This is the Javascript that turns HTML to VR content.

Tag Attributes

<a-sphere id="prettyNice" color="red" radius="4" position="1 -1 1"></a-sphere>

position: which is in the format of X, Y, Z- the 3 dimensions of space. Increasing Y for example moves up, decreasing moves down. Try changing them to see what happens!
color: which works the same as in the <a-sky>
radius: determines how big the sphere (our planet) is
id: this doesn't determine anything here, but it's a good way to let you know what the sphere is supposed to be and can be used to reference the sphere in more advanced A-Frame scenes

If we want two spheres together, wrap them in a tag called <a-entity>. 

<a-entity>
  <a-sphere id="wrappedUp" color="red" radius="4" position="1 -1 1"></a-sphere>
  <a-sphere id="wrappedUpTogether" color="blue" radius="4" position="0 -0 1"></a-sphere>
</a-entity>

Example
In order to create ringed planets, create rings with a shape called a "torus". Keep rings and planets in relative position with the <a-entity> tag.
  
  <a-entity id="saturn-container" position="4 2 -10">
                <a-sphere position="0 0 0 " radius=".8" color="#F8EC99" id="saturn"></a-sphere>
                <a-torus id="saturn-ring-1" color="#57524A" segments-tubular="50" radius="3.2" radius-tubular="0.1"
                    rotation="90 0 0" scale=".44 .44 0.04"></a-torus>
                <a-torus id="saturn-ring-2" color="#A29A87" segments-tubular="50" radius="2.4" radius-tubular="0.2"
                    rotation="90 0 0" scale=".44 .44 0.04"></a-torus>
            </a-entity>
