How do I import objects from my 3D app?
=======================================


Unity supports importing from most popular 3D applications. Choose the one you're working with below:

* [Maya](howto-importobjectmaya.html)
* [Cinema 4D](howto-importobjectcinema4d.html)
* [3ds Max](howto-importobjectmax.html)
* [Cheetah3D](howto-importobjectcheetah3d.html)
* [Modo](howto-importobjectmodo.html)
* [Lightwave](howto-importobjectlightwave.html)
* [Blender](howto-importobjectblender.html)

Other applications
------------------


Unity can read __.FBX__, __.dae__, __.3DS__, __.dxf__ and __.obj__ files, so check to see if your program can export to one of these formats. FBX exporters for popular 3D packages can be found [here](http://autodesk.com/fbx.html). Many packages also have a Collada exporter available.

Hints
-----


* Store textures in a folder called <span class=keyword>Textures</span> next to the exported mesh. This will guarantee that Unity will always be able to find the Texture and automatically connect the Texture to the Material. For more information, see the [Textures](class-texture2d.html) reference.

See Also
--------

* [Modeling Optimized Characters](modelingoptimizedcharacters.html)
* [How do I use normal maps?](howto-bumpmap.html)
* [Mesh Import Settings](class-mesh.html)
* [How do I fix the rotation of an imported model?](howto-fixzaxisisup.html)
