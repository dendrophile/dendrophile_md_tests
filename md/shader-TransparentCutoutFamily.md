Transparent Cutout Shader Family
================================


The Transparent Cutout shaders are used for objects that have fully opaque and fully transparent parts (no partial transparency). Things like chain fences, trees, grass, etc.

[Transparent Cutout Vertex-Lit](shader-transcutvertexlit.html)
--------------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutVertex.png](shader-transcutvertexlit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransCutVertexLit | &#187; More details](shader-transcutvertexlit|&#187;moredetails.html)


[Transparent Cutout Diffuse](shader-transcutdiffuse.html)
---------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutDiffuse.png](shader-transcutdiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransCutDiffuse | &#187; More details](shader-transcutdiffuse|&#187;moredetails.html)


[Transparent Cutout Specular](shader-transcutspecular.html)
-----------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutSpec.png](shader-transcutspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransCutSpecular | &#187; More details](shader-transcutspecular|&#187;moredetails.html)


[Transparent Cutout Bumped](shader-transcutbumpeddiffuse.html)
--------------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutBump.png](shader-transcutbumpeddiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-TransCutBumpedDiffuse | &#187; More details](shader-transcutbumpeddiffuse|&#187;moredetails.html)


[Transparent Cutout Bumped Specular](shader-transcutbumpedspecular.html)
------------------------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutBumpSpec.png](shader-transcutbumpedspecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransCutBumpedSpecular | &#187; More details](shader-transcutbumpedspecular|&#187;moredetails.html)


