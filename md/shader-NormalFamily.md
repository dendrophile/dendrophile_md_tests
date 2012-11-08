Normal Shader Family
====================


These shaders are the basic shaders in Unity.  They are not specialized in any way and should be suitable for most opaque objects.  They are not suitable if you want your object to be transparent, emitting light etc. 

[Vertex Lit](shader-NormalVertexLit.html)
-----------------------------------------


[Attach:Shaders./Thumb-NormalVertex.png](shader-NormalVertexLit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required


[Diffuse](shader-NormalDiffuse.html)
------------------------------------


[Attach:Shaders./Thumb-NormalDiffuse.png](shader-NormalDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required


[Specular](shader-NormalSpecular.html)
--------------------------------------


[Attach:Shaders./Thumb-NormalSpec.png](shader-NormalSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map


[Normal mapped](shader-NormalBumpedDiffuse.html)
------------------------------------------------


[Attach:Shaders./Thumb-NormalBump.png](shader-NormalBumpedDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Normal map</span>


[Normal mapped Specular](shader-NormalBumpedSpecular.html)
----------------------------------------------------------


[Attach:Shaders./Thumb-NormalBumpSpec.png](shader-NormalBumpedSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Normal map</span>


[Parallax](shader-NormalParallaxDiffuse.html)
---------------------------------------------


[Attach:Shaders./Thumb-NormalParallaxBump.png](shader-NormalParallaxDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Normal map</span>
* One <span class=component>Height</span> texture with Parallax Depth in the alpha channel


[Parallax Specular](shader-NormalParallaxSpecular.html)
-------------------------------------------------------


[Attach:Shaders./Thumb-NormalParallaxBumpSpec.png](shader-NormalParallaxSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Normal map</span>
* One <span class=component>Height</span> texture with Parallax Depth in the alpha channel


[Decal](shader-NormalDecal.html)
--------------------------------


[Attach:Shaders./Thumb-NormalDecal.png](shader-NormalDecal.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Decal</span> texture with alpha channel for Decal transparency


[Diffuse Detail](shader-NormalDiffuseDetail.html)
-------------------------------------------------


[Attach:Shaders./Thumb-NormalDiffuseDetail.png](shader-NormalDiffuseDetail.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Detail</span> grayscale texture; with 50% gray being neutral color
