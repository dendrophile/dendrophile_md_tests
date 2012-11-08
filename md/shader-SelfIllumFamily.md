Self-Illuminated Shader Family
==============================


The <span class=keyword>Self-Illuminated</span> shaders will emit light only onto themselves based on an attached alpha channel.  They do not require any Lights to shine on them to emit this light.  Any vertex lights or pixel lights will simply add more light on top of the self-illumination.

This is mostly used for light emitting objects. For example, parts of the wall texture could be self-illuminated to simulate lights or displays.  It can also be useful to light power-up objects that should always have consistent lighting throughout the game, regardless of the lights shining on it.

[Self-Illuminated Vertex-Lit](shader-selfillumvertexlit.html)
-------------------------------------------------------------


[Attach:Shaders./Thumb-IllumVertex.png](shader-selfillumvertexlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Illumination</span> texture with alpha channel for Illumination Map

[shader-SelfIllumVertexLit| &#187; More details](shader-selfillumvertexlit|&#187;moredetails.html)


[Self-Illuminated Diffuse](shader-selfillumdiffuse.html)
--------------------------------------------------------


[Attach:Shaders./Thumb-IllumDiffuse.png](shader-selfillumdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Illumination</span> texture with alpha channel for Illumination Map

[shader-SelfIllumDiffuse | &#187; More details](shader-selfillumdiffuse|&#187;moredetails.html)


[Self-Illuminated Specular](shader-selfillumspecular.html)
----------------------------------------------------------


[Attach:Shaders./Thumb-IllumSpec.png](shader-selfillumspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Illumination</span> texture with alpha channel for Illumination Map

[shader-SelfIllumSpecular | &#187; More details](shader-selfillumspecular|&#187;moredetails.html)


[Self-Illuminated Bumped](shader-selfillumbumpeddiffuse.html)
-------------------------------------------------------------


[Attach:Shaders./Thumb-IllumBump.png](shader-selfillumbumpeddiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Normal map</span> normal map with alpha channel for Illumination

[shader-SelfIllumBumpedDiffuse | &#187; More details](shader-selfillumbumpeddiffuse|&#187;moredetails.html)


[Self-Illuminated Bumped Specular](shader-selfillumbumpedspecular.html)
-----------------------------------------------------------------------


[Attach:Shaders./Thumb-IllumBumpSpec.png](shader-selfillumbumpedspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Normal map</span> normal map with alpha channel for Illumination Map

[shader-SelfIllumBumpedSpecular | &#187; More details](shader-selfillumbumpedspecular|&#187;moredetails.html)


[Self-Illuminated Parallax](shader-selfillumparallaxdiffuse.html)
-----------------------------------------------------------------


[Attach:Shaders./Thumb-IllumParallaxBump.png](shader-selfillumparallaxdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture, no alpha channel required
* One <span class=component>Normal map</span> normal map with alpha channel for Illumination Map & Parallax Depth combined

_'Note:_'
One consideration of this shader is that the <span class=component>Bumpmap</span> texture's alpha channel doubles as a Illumination and the Parallax Depth.

[shader-SelfIllumParallaxDiffuse | &#187; More details](shader-selfillumparallaxdiffuse|&#187;moredetails.html)


[Self-Illuminated Parallax Specular](shader-selfillumparallaxspecular.html)
---------------------------------------------------------------------------


[Attach:Shaders./Thumb-IllumParallaxBumpSpec.png](shader-selfillumparallaxspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Specular Map
* One <span class=component>Normal map</span> normal map with alpha channel for Illumination Map & Parallax Depth combined

_'Note:_'
One consideration of this shader is that the <span class=component>Bumpmap</span> texture's alpha channel doubles as a Illumination and the Parallax Depth.

[shader-SelfIllumParallaxSpecular | &#187; More details](shader-selfillumparallaxspecular|&#187;moredetails.html)
