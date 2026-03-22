# Tool Learning Log

## Tool: **A-frame**

---
 I've been using loose-leaf to take notes on the topics I'm learning from A-frame, then I will be typing the notes in here!
### 3/16/26:
* What is A-Frame: It's a Web framework for virtual reality experiences. A-frame is based on HTML.
* Just drop in a `<script>` tag and a `<a-scene>`. So A-frame handles 3d boiler plate, the VR setup, and default controls.
* A frame has a handy built in 3d inspector so when you open a-frame scene and hit ctrl+i or ctrl+option+i
* They have core components like
    * Geometries
    * Materials
    * Lights
    * animations
    * models
    * raycasters
    * shadows
    * positonal
    * audio
    * text
* They have components like furthermore
    * environment
    * state
    * particle systems
    * physics
    * multiuser
    * oceans
    * teleportation
    * augmented reality

### 3/17/2026
* Installation + Testing: Go to A-Frame documentation and copy the script, paste it inside the head tag
* When you add the a-scene element, it enters the VR mode button, telling you it has been installed
* Basic Primitives + HTML attributes are in the documentation
* Each primitive has its own specific attributes + properties


### 3/18/26:
What I learned while reading through the **entity component system** doc on A-Frame
* ECS architecture is a common desirable pattern in 3D and game development that is led by the composition over inheritance and hierarchy principle.
* An entity is basically a mix of components that assemble to create an entity, for example, from the documentation says Light **Bulb = Position + Light + Geometry + Material + Shadow**
* Systems are represented by <a-scene>‘s HTML attributes.
* To create an entity, we can use this format
* format: <a-entity ${componentName}="${propertyName1}: ${propertyValue1}; ${propertyName2}: ${propertyValue2}">
What I learned while reading through the **writing a compoent** doc on A-Frame
### 3/19/26:
* Text

### 3/20/26:
* Text
### 3/21/26:
* Text
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
