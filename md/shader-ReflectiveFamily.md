Reflective Shader Family
========================


<span class=keyword>Reflective</span> shaders will allow you to use a Cubemap which will be reflected on your mesh.  You can also define areas of more or less reflectivity on your object through the alpha channel of the <span class=component>Base</span> texture. High relectivity is a great effect for glosses, oils, chrome, etc.  Low reflectivity can add effect for metals, liquid surfaces, or video monitors.

[Reflective Vertex-Lit](shader-ReflectiveVertexLit.html)
--------------------------------------------------------


[Attach:Shaders./Thumb-ReflVertex.png](shader-ReflectiveVertexLit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map

[shader-ReflectiveVertexLit | &#187; More details](shader-ReflectiveVertexLit|&#187;Moredetails.html)


[Reflective Diffuse](shader-ReflectiveDiffuse.html)
---------------------------------------------------


[Attach:Shaders./Thumb-ReflDiffuse.png](shader-ReflectiveDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map

[shader-ReflectiveDiffuse | &#187; More details](shader-ReflectiveDiffuse|&#187;Moredetails.html)


[Reflective Specular](shader-ReflectiveSpecular.html)
-----------------------------------------------------


[Attach:Shaders./Thumb-ReflSpec.png](shader-ReflectiveSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas & Specular Map combined
* One <span class=component>Reflection</span> Cubemap for Reflection Map

_'Note:_'
One consideration for this shader is that the <span class=component>Base</span> texture's alpha channel will double as both the reflective areas and the Specular Map.

[shader-ReflectiveSpecular | &#187; More details](shader-ReflectiveSpecular|&#187;Moredetails.html)


[Reflective Normal mapped](shader-ReflectiveBumpedDiffuse.html)
---------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBump.png](shader-ReflectiveBumpedDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-ReflectiveBumpedDiffuse | &#187; More details](shader-ReflectiveBumpedDiffuse|&#187;Moredetails.html)


[Reflective Normal Mapped Specular](shader-ReflectiveBumpedSpecular.html)
-------------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBumpSpec.png](shader-ReflectiveBumpedSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas & Specular Map combined
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

_'Note:_'
One consideration for this shader is that the <span class=component>Base</span> texture's alpha channel will double as both the reflective areas and the Specular Map.

[shader-ReflectiveBumpedSpecular | &#187; More details](shader-ReflectiveBumpedSpecular|&#187;Moredetails.html)


[Reflective Parallax](shader-ReflectiveParallaxDiffuse.html)
------------------------------------------------------------


[Attach:Shaders./Thumb-ReflParallaxBump.png](shader-ReflectiveParallaxDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, with alpha channel for Parallax Depth

[shader-ReflectiveParallaxDiffuse | &#187; More details](shader-ReflectiveParallaxDiffuse|&#187;Moredetails.html)


[Reflective Parallax Specular](shader-ReflectiveParallaxSpecular.html)
----------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflParallaxBumpSpec.png](shader-ReflectiveParallaxSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas & Specular Map
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, with alpha channel for Parallax Depth

_'Note:_'
One consideration for this shader is that the <span class=component>Base</span> texture's alpha channel will double as both the reflective areas and the Specular Map.

[shader-ReflectiveParallaxSpecular | &#187; More details](shader-ReflectiveParallaxSpecular|&#187;Moredetails.html)


[Reflective Normal mapped Unlit](shader-ReflectiveBumpedUnlit.html)
-------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBumpUnlit.png](shader-ReflectiveBumpedUnlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-ReflectiveBumpedUnlit | &#187; More details](shader-ReflectiveBumpedUnlit|&#187;Moredetails.html)


[Reflective Normal mapped Vertex-Lit](shader-ReflectiveBumpedVertexLit.html)
----------------------------------------------------------------------------


[Attach:Shaders./Thumb-ReflBumpVertex.png](shader-ReflectiveBumpedVertexLit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for defining reflective areas
* One <span class=component>Reflection</span> Cubemap for Reflection Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-ReflectiveBumpedVertexLit | &#187; More details](shader-ReflectiveBumpedVertexLit|&#187;Moredetails.html)
