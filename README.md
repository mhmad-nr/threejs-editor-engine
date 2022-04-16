Engine ES Mode
===========

## Editor/Simulator WebApp

http://tfs/nechi/control-3d-v5 Core

[HTML5 ¿SWAC CWC?] 

### Main entry
http://tfs/nechi/threejs-editor-engine/index.html

### Storage (indexedDB)
http://tfs/nechi/threejs-editor-engine/js/Storage.js
### Editor
http://tfs/nechi/threejs-editor-engine/js/Editor.js
### Player
http://tfs/nechi/threejs-editor-engine/js/Player.js
### Signals API
http://tfs/nechi/threejs-editor-engine/js/Editor.js#L14
### Scripting UI
http://tfs/nechi/threejs-editor-engine/js/Script.js
#### Code Mirror Scripting Editor
    CodeMirror is a versatile text editor implemented in JavaScript for the browser. It is specialized for editing code, and comes with a number of language modes and addons that implement more advanced editing functionality.

    A rich programming API and a CSS theming system are available for customizing CodeMirror to fit your application, and extending it with new functionality.

Tern.js Intelligent/ Acorn.js Scripting Parser / esprima.js ECMAScript parsing  
    http://tfs/nechi/threejs-editor-engine/js/libs/tern-engine/engine.js

#### Under-the-hoods 
[DOM 2 THREEjs][DOM 2 Canvas] [JSON lint] UIg
            
http://tfs/nechi/threejs-editor-engine/js/libs/ui.js  
http://tfs/nechi/threejs-editor-engine/js/libs/ui.three.js  
http://tfs/nechi/threejs-editor-engine/js/libs/html2canvas.js  
http://tfs/nechi/threejs-editor-engine/js/libs/jsonlint.js  

    Shaders use GLSL (OpenGL Shading Language), a special OpenGL Shading Language with syntax   similar to C
http://tfs/nechi/threejs-editor-engine/js/libs/codemirror/mode/glsl.js

## Enginering Simulator WebApp
[HTML5 ¿SWAC CWC?] 
Enginering Simulator app.

http://tfs/nechi/control-3d-v5 Core

¿SWAC Interface?

### Main entry
http://tfs/nechi/threejs-editor-engine/js/libs/engine/index.html
http://tfs/nechi/threejs-editor-engine/js/libs/engine.js

### UnityWebGL Player
A WebApp to present Unity WebGL Player.  
http://tfs/nechi/control-3d-unity-webgl-screen/index.html

### glTF 2 UnityScene driver
A wraper to handle loading of glTF model files from javascript into Unity WebGL Player.  
http://tfs/nechi/control-3d-unity-webgl-object-model

Three.js Editor - Engine Version
================
This repository contains the 3D editor extracted from [threejs-editor.js](https://github.com/nterms/threejs-editor)


Three.js Editor
==============

This repository contains the 3D editor extracted from [three.js](https://github.com/mrdoob/three.js)


Signals API
--------------
http://tfs/nechi/threejs-editor-engine/js/Editor.js#L14

```js
// script

editScript: new Signal(),

// player

startPlayer: new Signal(),
stopPlayer: new Signal(),

// actions

showModal: new Signal(),

// notifications

editorCleared: new Signal(),

savingStarted: new Signal(),
savingFinished: new Signal(),

themeChanged: new Signal(),

transformModeChanged: new Signal(),
snapChanged: new Signal(),
spaceChanged: new Signal(),
rendererChanged: new Signal(),

sceneBackgroundChanged: new Signal(),
sceneFogChanged: new Signal(),
sceneGraphChanged: new Signal(),

cameraChanged: new Signal(),

geometryChanged: new Signal(),

objectSelected: new Signal(),
objectFocused: new Signal(),

objectAdded: new Signal(),
objectChanged: new Signal(),
objectRemoved: new Signal(),

helperAdded: new Signal(),
helperRemoved: new Signal(),

materialChanged: new Signal(),

scriptAdded: new Signal(),
scriptChanged: new Signal(),
scriptRemoved: new Signal(),

windowResize: new Signal(),

showGridChanged: new Signal(),
refreshSidebarObject3D: new Signal(),
historyChanged: new Signal()

```