ShaderLab syntax: other commands
================================


Category
--------


__Category__ is a logical grouping of any commands below it. This is mostly used to "inherit" rendering state. For example, your shader might have multiple [subshaders](sl-subshader.html), and each of them requires [fog](sl-fog.html) to be off, [blending](sl-blend.html) set to additive, etc. You can use Category for that:
````

Shader "example" {
Category {
    Fog { Mode Off }
    Blend One One
    SubShader {
        // ...
    }
    SubShader {
        // ...
    }
    // ...
}
}

````

Category block only affects shader parsing, it's exactly the same as "pasting" any state set inside Category into all blocks below it. It does not affect shader execution speed at all.

