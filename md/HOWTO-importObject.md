How do I import objects from my 3D app?
=======================================


Unity supports importing from most popular 3D applications. Choose the one you're working with below:

* [Maya](HOWTO-ImportObjectMaya.html)
* [Cinema 4D](HOWTO-ImportObjectCinema4D.html)
* [3ds Max](HOWTO-ImportObjectMax.html)
* [Cheetah3D](HOWTO-ImportObjectCheetah3D.html)
* [Modo](HOWTO-ImportObjectModo.html)
* [Lightwave](HOWTO-importObjectLightwave.html)
* [Blender](HOWTO-ImportObjectBlender.html)

Other applications
------------------


Unity can read __.FBX__, __.dae__, __.3DS__, __.dxf__ and __.obj__ files, so check to see if your program can export to one of these formats. FBX exporters for popular 3D packages can be found [here](http://autodesk.com/fbx.html). Many packages also have a Collada exporter available.

Hints
-----


* Store textures in a folder called <span class=keyword>Textures</span> next to the exported mesh. This will guarantee that Unity will always be able to find the Texture and automatically connect the Texture to the Material. For more information, see the [Textures](class-Texture2D.html) reference.

See Also
--------

* [Modeling Optimized Characters](ModelingOptimizedCharacters.html)
* [How do I use normal maps?](HOWTO-bumpmap.html)
* [Mesh Import Settings](class-Mesh.html)
* [How do I fix the rotation of an imported model?](HOWTO-FixZAxisIsUp.html)
