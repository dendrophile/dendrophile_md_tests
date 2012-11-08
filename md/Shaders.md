Shaders
=======


All rendering in Unity is done with _Shaders_ - small scripts that let you configure the how the graphics hardware is set up for rendering. Unity ships with 60+ built-in shaders (documented in the [Built-in Shader Guide](Built-inShaderGuide.html)). You can extend this by making your own shaders. 

Shaders in Unity can be written in one of three different ways:

###Surface Shaders

[Surface Shaders](SL-SurfaceShaders.html) are your best option _if your shader needs to be affected by lights and shadows_. Surface shaders make it easy to write complex shaders in a compact way - it's a higher level of abstraction for interaction with Unity's lighting pipeline. Most surface shaders automatically support both forward and deferred lighting. You write surface shaders in a couple of lines of __Cg/HLSL__ and a lot more code gets auto-generated from that.

Do _not_ use surface shaders if your shader is not doing anything with lights. For [Image Effects](comp-ImageEffects.html) or many special-effect shaders, surface shaders are a suboptimal option, since they will do a bunch of lighting calculations for no good reason!


###Vertex and Fragment Shaders

Vertex and Fragment Shaders will be required, if your shader doesn't need to interact with lighting, or if you need some very exotic effects that the surface shaders can't handle. Shader programs written this way are the most flexible way to create the effect you need (even surface shaders are automatically converted to a bunch of vertex and fragment shaders), but that comes at a price: you have to write more code and it's harder to make it interact with lighting. These shaders are written in __Cg/HLSL__ as well.


###Fixed Function Shaders

Fixed Function Shaders need to be written for old hardware that doesn't support programmable shaders. You will probably want to write fixed function shaders as an n-th fallback to your fancy fragment or surface shaders, to make sure your game still renders something sensible when run on old hardware or simpler mobile platforms. Fixed function shaders are entirely written in a language called __ShaderLab__, which is similar to Microsoft's .FX files or NVIDIA's CgFX.


ShaderLab
---------


Regardless of which type you choose, the actual meat of the shader code will always be wrapped in ShaderLab, which is used to organize the shader structure. It looks like this:

````
Shader "MyShader" {
    Properties {
        _MyTexture ("My Texture", 2D) = "white" { }
        // other properties like colors or vectors go here as well
    }
    SubShader {
        // here goes the 'meat' of your
        //  - surface shader or
        //  - vertex and fragment shader or
        //  - fixed function shader
    }
    SubShader {
        // here goes a simpler version of the SubShader above that can run on older graphics cards
    }
} 
````

We recommend that you start by reading about some basic concepts of the ShaderLab syntax in the [ShaderLab reference](SL-Shader.html) and then move on to the tutorials listed below.

The tutorials include plenty of examples for the different types of shaders. For even more examples of surface shaders in particular, you can get the source of Unity's built-in shaders from the [Resources section](http://www.unity3d.com/support/resources/assets/built-in-shaders.html). Unity's [Image Effects](comp-ImageEffects.html) package contains a lot of interesting vertex and fragment shaders.

Read on for an introduction to shaders, and check out the [shader reference](SL-Reference.html)!

* [Tutorial: ShaderLab & Fixed Function Shaders](ShaderTut1.html)
* [Tutorial: Vertex and Fragment Shaders](ShaderTut2.html)
* [Surface Shaders](SL-SurfaceShaders.html)