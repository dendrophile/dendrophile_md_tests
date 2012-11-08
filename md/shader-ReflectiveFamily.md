Reflective Shader Family
========================


<span class=keyword>Reflective</span> shaders will allow you to use a Cubemap which will be reflected on your mesh.  You can also define areas of more or less reflectivity on your object through the alpha channel of the <span class=component>Base</span> texture. High relectivity is a great effect for glosses, oils, chrome, etc.  Low reflectivity can add effect for metals, liquid surfaces, or video monitors.

[Reflective Vertex-Lit](shader-reflectivevertexlit.html)
--------------------------------------------------------


[Attach:Shaders./Thumb-ReflVertex.png](shader-reflectivevertexlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map

[shader-ReflectiveVertexLit | &#187; More details](shader-reflectivevertexlit|&#187;moredetails.html)


[Reflective Diffuse](shader-reflectivediffuse.html)
---------------------------------------------------


[Attach:Shaders./Thumb-ReflDiffuse.png](shader-reflectivediffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map

[shader-ReflectiveDiffuse | &#187; More details](shader-reflectivediffuse|&#187;moredetails.html)


[Reflective Specular](shader-reflectivespecular.html)
-----------------------------------------------------


[Attach:Shaders./Thumb-ReflSpec.png](shader-reflectivespecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas & Specular Map combined
* One <span class=component>Reflection</span> Cubemap for Reflection Map

_'Note:_'
One consideration for this shader is that the <span class=component>Base</span> texture's alpha channel will double as both the reflective areas and the Specular Map.

[shader-ReflectiveSpecular | &#187; More details](shader-reflectivespecular|&#187;moredetails.html)


[Reflective Normal mapped](shader-reflectivebumpeddiffuse.html)
---------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBump.png](shader-reflectivebumpeddiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-ReflectiveBumpedDiffuse | &#187; More details](shader-reflectivebumpeddiffuse|&#187;moredetails.html)


[Reflective Normal Mapped Specular](shader-reflectivebumpedspecular.html)
-------------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBumpSpec.png](shader-reflectivebumpedspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas & Specular Map combined
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

_'Note:_'
One consideration for this shader is that the <span class=component>Base</span> texture's alpha channel will double as both the reflective areas and the Specular Map.

[shader-ReflectiveBumpedSpecular | &#187; More details](shader-reflectivebumpedspecular|&#187;moredetails.html)


[Reflective Parallax](shader-reflectiveparallaxdiffuse.html)
------------------------------------------------------------


[Attach:Shaders./Thumb-ReflParallaxBump.png](shader-reflectiveparallaxdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, with alpha channel for Parallax Depth

[shader-ReflectiveParallaxDiffuse | &#187; More details](shader-reflectiveparallaxdiffuse|&#187;moredetails.html)


[Reflective Parallax Specular](shader-reflectiveparallaxspecular.html)
----------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflParallaxBumpSpec.png](shader-reflectiveparallaxspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas & Specular Map
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, with alpha channel for Parallax Depth

_'Note:_'
One consideration for this shader is that the <span class=component>Base</span> texture's alpha channel will double as both the reflective areas and the Specular Map.

[shader-ReflectiveParallaxSpecular | &#187; More details](shader-reflectiveparallaxspecular|&#187;moredetails.html)


[Reflective Normal mapped Unlit](shader-reflectivebumpedunlit.html)
-------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBumpUnlit.png](shader-reflectivebumpedunlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-ReflectiveBumpedUnlit | &#187; More details](shader-reflectivebumpedunlit|&#187;moredetails.html)


[Reflective Normal mapped Vertex-Lit](shader-reflectivebumpedvertexlit.html)
----------------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBumpVertex.png](shader-reflectivebumpedvertexlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-ReflectiveBumpedVertexLit | &#187; More details](shader-reflectivebumpedvertexlit|&#187;moredetails.html)
