Normal Shader Family
====================


These shaders are the basic shaders in Unity.  They are not specialized in any way and should be suitable for most opaque objects.  They are not suitable if you want your object to be transparent, emitting light etc. 

[Vertex Lit](shader-normalvertexlit.html)
-----------------------------------------


[Attach:Shaders./Thumb-NormalVertex.png](shader-normalvertexlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required


[Diffuse](shader-normaldiffuse.html)
------------------------------------


[Attach:Shaders./Thumb-NormalDiffuse.png](shader-normaldiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required


[Specular](shader-normalspecular.html)
--------------------------------------


[Attach:Shaders./Thumb-NormalSpec.png](shader-normalspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map


[Normal mapped](shader-normalbumpeddiffuse.html)
------------------------------------------------


[Attach:Shaders./Thumb-NormalBump.png](shader-normalbumpeddiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Normal map</span>


[Normal mapped Specular](shader-normalbumpedspecular.html)
----------------------------------------------------------


[Attach:Shaders./Thumb-NormalBumpSpec.png](shader-normalbumpedspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Normal map</span>


[Parallax](shader-normalparallaxdiffuse.html)
---------------------------------------------


[Attach:Shaders./Thumb-NormalParallaxBump.png](shader-normalparallaxdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Normal map</span>
* One <span class=component>Height</span> texture with Parallax Depth in the alpha channel


[Parallax Specular](shader-normalparallaxspecular.html)
-------------------------------------------------------


[Attach:Shaders./Thumb-NormalParallaxBumpSpec.png](shader-normalparallaxspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Normal map</span>
* One <span class=component>Height</span> texture with Parallax Depth in the alpha channel


[Decal](shader-normaldecal.html)
--------------------------------


[Attach:Shaders./Thumb-NormalDecal.png](shader-normaldecal.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Decal</span> texture with alpha channel for Decal transparency


[Diffuse Detail](shader-normaldiffusedetail.html)
-------------------------------------------------


[Attach:Shaders./Thumb-NormalDiffuseDetail.png](shader-normaldiffusedetail.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Detail</span> grayscale texture; with 50% gray being neutral color
