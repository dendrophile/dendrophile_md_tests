Transparent Cutout Shader Family
================================


The Transparent Cutout shaders are used for objects that have fully opaque and fully transparent parts (no partial transparency). Things like chain fences, trees, grass, etc.

[Transparent Cutout Vertex-Lit](shader-TransCutVertexLit.html)
--------------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutVertex.png](shader-TransCutVertexLit.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransCutVertexLit | &#187; More details](shader-TransCutVertexLit|&#187;Moredetails.html)


[Transparent Cutout Diffuse](shader-TransCutDiffuse.html)
---------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutDiffuse.png](shader-TransCutDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map

[shader-TransCutDiffuse | &#187; More details](shader-TransCutDiffuse|&#187;Moredetails.html)


[Transparent Cutout Specular](shader-TransCutSpecular.html)
-----------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutSpec.png](shader-TransCutSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransCutSpecular | &#187; More details](shader-TransCutSpecular|&#187;Moredetails.html)


[Transparent Cutout Bumped](shader-TransCutBumpedDiffuse.html)
--------------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutBump.png](shader-TransCutBumpedDiffuse.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for Transparency Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

[shader-TransCutBumpedDiffuse | &#187; More details](shader-TransCutBumpedDiffuse|&#187;Moredetails.html)


[Transparent Cutout Bumped Specular](shader-TransCutBumpedSpecular.html)
------------------------------------------------------------------------


[Attach:Shaders./Thumb-TransCutoutBumpSpec.png](shader-TransCutBumpedSpecular.html)

_'Assets needed:_'
* One <span class=component>Base</span> texture with alpha channel for combined Transparency Map/Specular Map
* One <span class=component>Normal map</span> normal map, no alpha channel required

_'Note:_'
One limitation of this shader is that the <span class=component>Base</span> texture's alpha channel doubles as a Specular Map for the Specular shaders in this family.

[shader-TransCutBumpedSpecular | &#187; More details](shader-TransCutBumpedSpecular|&#187;Moredetails.html)


