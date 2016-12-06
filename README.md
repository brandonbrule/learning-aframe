# learning-aframe
Quick Talk on A-Frame for #CodePenOttawa


1. Sky
2. Shapes (pos, size, rot)
3. Textures (src & asset loading)
4. Lighting
5. Animate
6. Dynamic Elements
7. Voxel Models
8. PlaceIt


## Source
First Load Up to Source
https://aframe.io/releases/0.3.0/aframe.min.js


##a-scene
The wrapper around the Aframe

Aframe Units of Measurement is in Meters.
A box with height="100" may look ordinary on our computer screens, but in virtual reality it will look massive.



##Sky
Equirectangular Projection Backgrounds
A simple map projection attributed to Marinus of Tyre, who Ptolemy claims invented the projection about AD 100
Background attached to the entire scene
Image or Background Color
<a-sky src="sky.png"></a-sky>
<a-sky color="red"></a-sky>

You could also attach a background image/gradient to the body element.



##Shapes
Aframe build in object primitives:
https://aframe.io/docs/0.3.0/components/geometry.html

To start, everything rendered is nested in <a-scene>

Primitives are custom html elements that render premade shapes.
<a box></a-box>

Attributes control things like position, rotation, and color/texture.
Position="x y z"
Rotation="x y z"
height, width, depth = "m"



##Textures
Textures can be applied as a standard src attribute on the a-frame primitives.
src="imagepath/img.png"

Best practices and when working with larger amounts of data there is an asset a-frame element that can preload all of your textures before rendering out.
https://aframe.io/docs/0.3.0/core/asset-management-system.html



##Lighting
I only had luck with the default <a-light> element which is like a source from the sun.  You can control it's position and colour in the sky casting different shadows across your scene.
https://aframe.io/docs/0.3.0/components/light.html http://localhost/www/aframe/4-lighting/


##Animations
We can animate each entity by nesting a custom animation element inside an a-entity element.  The animation property names are influenced by CSS animations and supports animating things like color, position, opacity, delays, duration, and number of repeats.


##Dynamic
We can dynamically create a-frame elements like any regular html element.  we can setAttributes, and created nested animations and append it to the scene on some action.


##External Models
This is a little town that was built in a voxel editing program VoxelMagica, It's been imported into a-frame and we can move around and add lighting to the scene that holds the model.


##Place It.
Tiny little scene builder


Extras
https://github.com/donmccurdy/aframe-extras
