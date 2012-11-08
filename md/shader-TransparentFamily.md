Transparent Shader Family
=========================


The Transparent shaders are used for fully- or semi-transparent objects.  Using the alpha channel of the <span class=component>Base</span> texture, you can determine areas of the object which can be more or less transparent than others.  This can create a great effect for glass, HUD interfaces, or sci-fi effects.

[Transparent Vertex-Lit](shader-TransVertexLit.html)
----------------------------------------------------


[Attach:Shaders./Thumb-TransVertex.png](shader-TransVertexLit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransVertexLit | &#187; More details](shader-TransVertexLit|&#187;Moredetails.html)


[Transparent Diffuse](shader-TransDiffuse.html)
-----------------------------------------------


[Attach:Shaders./Thumb-TransDiffuse.png](shader-TransDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransDiffuse | &#187; More details](shader-TransDiffuse|&#187;Moredetails.html)


[Transparent Specular](shader-TransSpecular.html)
-------------------------------------------------


[Attach:Shaders./Thumb-TransSpec.png](shader-TransSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.


[shader-TransSpecular | &#187; More details](shader-TransSpecular|&#187;Moredetails.html)


[Transparent Normal mapped](shader-TransBumpedDiffuse.html)
-----------------------------------------------------------


[Attach:Shaders./Thumb-TransBump.png](shader-TransBumpedDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-TransBumpedDiffuse | &#187; More details](shader-TransBumpedDiffuse|&#187;Moredetails.html)


[Transparent Normal mapped Specular](shader-TransBumpedSpecular.html)
---------------------------------------------------------------------


[Attach:Shaders./Thumb-TransBumpSpec.png](shader-TransBumpedSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransBumpedSpecular | &#187; More details](shader-TransBumpedSpecular|&#187;Moredetails.html)


[Transparent Parallax](shader-TransParallaxDiffuse.html)
--------------------------------------------------------


[Attach:Shaders./Thumb-TransParallaxBump.png](shader-TransParallaxDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map
* One <span class=component>Normal map</span> normal map with alpha channel for Parallax Depth

[shader-TransParallaxDiffuse | &#187; More details](shader-TransParallaxDiffuse|&#187;Moredetails.html)


[Transparent Parallax Specular](shader-TransParallaxSpecular.html)
------------------------------------------------------------------


[Attach:Shaders./Thumb-TransParallaxBumpSpec.png](shader-TransParallaxSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map
* One <span class=component>Normal map</span> normal map with alpha channel for Parallax Depth

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransParallaxSpecular | &#187; More details](shader-TransParallaxSpecular|&#187;Moredetails.html)
