Transparent Shader Family
=========================


The Transparent shaders are used for fully- or semi-transparent objects.  Using the alpha channel of the <span class=component>Base</span> texture, you can determine areas of the object which can be more or less transparent than others.  This can create a great effect for glass, HUD interfaces, or sci-fi effects.

[Transparent Vertex-Lit](shader-transvertexlit.html)
----------------------------------------------------


[Attach:Shaders./Thumb-TransVertex.png](shader-transvertexlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransVertexLit | &#187; More details](shader-transvertexlit|&#187;moredetails.html)


[Transparent Diffuse](shader-transdiffuse.html)
-----------------------------------------------


[Attach:Shaders./Thumb-TransDiffuse.png](shader-transdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransDiffuse | &#187; More details](shader-transdiffuse|&#187;moredetails.html)


[Transparent Specular](shader-transspecular.html)
-------------------------------------------------


[Attach:Shaders./Thumb-TransSpec.png](shader-transspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.


[shader-TransSpecular | &#187; More details](shader-transspecular|&#187;moredetails.html)


[Transparent Normal mapped](shader-transbumpeddiffuse.html)
-----------------------------------------------------------


[Attach:Shaders./Thumb-TransBump.png](shader-transbumpeddiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-TransBumpedDiffuse | &#187; More details](shader-transbumpeddiffuse|&#187;moredetails.html)


[Transparent Normal mapped Specular](shader-transbumpedspecular.html)
---------------------------------------------------------------------


[Attach:Shaders./Thumb-TransBumpSpec.png](shader-transbumpedspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransBumpedSpecular | &#187; More details](shader-transbumpedspecular|&#187;moredetails.html)


[Transparent Parallax](shader-transparallaxdiffuse.html)
--------------------------------------------------------


[Attach:Shaders./Thumb-TransParallaxBump.png](shader-transparallaxdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map
* One <span class=component>Normal map</span> normal map with alpha channel for Parallax Depth

[shader-TransParallaxDiffuse | &#187; More details](shader-transparallaxdiffuse|&#187;moredetails.html)


[Transparent Parallax Specular](shader-transparallaxspecular.html)
------------------------------------------------------------------


[Attach:Shaders./Thumb-TransParallaxBumpSpec.png](shader-transparallaxspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map
* One <span class=component>Normal map</span> normal map with alpha channel for Parallax Depth

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransParallaxSpecular | &#187; More details](shader-transparallaxspecular|&#187;moredetails.html)
