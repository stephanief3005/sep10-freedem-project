# Tool Learning Log

## Tool: **A-frame**

---
3/22/2026 note
 I've been using loose-leaf to take notes on the topics I'm learning from A-frame, and then I will be typing the notes in here!
 I feel like ive mostly took notes because i dont like doing something before learning it, so I think I will be working on practicing it more, since thats also learning too, so more tinkering rather than notes.
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
What I learned while reading through the **writing a component** doc on A-Frame
* Entities are like empty containers; they only have stuff added when components have been attached
* It's mostly good in use for complex objects with the formation of components by itself

### 3/19/26:
 Visual Inspector & Dev Tools
- ctrl + alt + i --> to inspect
- The inspector can be used to select, search, delete, clone, and add entities or export HTML.
- The viewport shows inspectors pov, so we can rotate, pan, or zoom the viewport to change the view of the scene, so you can transform entities, and it is better to use than switching back to code
- The viewport tools allow you to rotate, pan, zoom, select, and transform those entities using 3d handles
- There's a spectator mode for the third-person camera
- This is mostly used for testing, and better
- You can record

### 3/20/26:
Best Practices from A-frame
* Examples of what not to do
``` html
Do not do this:

<a-scene>
  <a-box></a-box>
  <!-- ... -->
</a-scene>

<script>
  // My JavaScript code here!
  // ... NO!
</script>
```
* what to do
``` html
<script>
  AFRAME.registerComponent('code-that-does-this', {
    init: function () {
      // Code here.
      console.log(this.el);
    }
  });

  AFRAME.registerComponent('code-to-attach-to-box', {
    init: function () {
      // Code here.
      console.log(this.el);
    }
  });
</script>

<a-scene code-that-does-this>
  <a-box code-to-attach-to-box></a-box>
  <!-- ... -->
</a-scene>
```
* Use VR design principles
* reduce unnecessary object creation
### 3/21/26:
Writing a component doc and takeaways
- Components can be reusable
- AFRAME.registerComponent() is used to register components
- Reusing components can help prevent performance issues
* Planning on what I want to use A-frame
  - I want to use it, so the future innovation I think may exist in the future is the electric floss so then
  - I would use components like cube and sphere mostly
  - I'd use the entity component system I learned on 3/18/26
### 3/23/26
**Introduction**
* Developed from plain html
- withour having to install
* A-FRAME is a web frame work for building virtual reality (VR) experiences
* the core is a poweful entity component framework that provides a declarative extensible and composable structure to three.js
* based on html
Drop in a `<script>` tag and `<a-scene>`. It will handle 3D boilet plate, VR set up and default controls
Powerful three.js framework, provides a declarative composable , reusable tntity component structure
- giving developers acccess to have unlimited access to Javascript, DOM, APIS , three js, webVR , Web GL
* You can build VR for Vive, Rift, Meta quest, windows mixed reality, and apple vission pro but im going to be using the standard desktop + smartphones
* 3D inspector Aframe scene with `<ctrl>` + alt + i or `<ctrl>` + option + i
so you can fly around to peek under the hood
and lastly for **components** can be checked in the documentation
**Installation**
**VR Headsets & WebXR Browsers**

Testing out:

### 3/24/26
**VR Headsets & WebXR Browsers**
**HTML & Primitives**
**Entity-Component-System**

### 3/25/26
**JavaScript, Events, DOM APIs**
**Developing with three.js**

### 3/26/26
**Writing a Component**
**Interactions & Controllers**

### 3/27/26
**3D Models**
**Visual Inspector & Dev Tools**

### 3/28/26
**Hosting & Publishing**
**Best Practices**
**Building a Basic Scene (Guide)**
**entity + component**

<!--
* Links you used today (websites, videos, etc.)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
