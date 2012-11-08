Troubleshooting Shadows
=======================


This page lists solutions to common [shadow](shadows.html) problems.

###I see no shadows at all!

* Shadows are a <span class=keyword>Unity Pro</span> only feature, so without Unity Pro you won't get shadows. Simpler shadow methods, like using a [Projector](class-projector.html), are still possible of course.
* Shadows also require certain graphics hardware support. See [Shadows](shadows.html) page for details.
* Check if shadows are not completely disabled in [Quality Settings](class-qualitysettings.html).
* __Shadows are currently not supported for iOS and Android mobile platforms.__

###Some of my objects do not cast or receive shadows

First, the [Renderer](class-meshrenderer.html) has to have <span class=component>Receive Shadows</span> on to have shadows on itself; and <span class=component>Cast Shadows</span> on to cast shadows on other objects (both are on by default).

Next, only opaque objects cast and receive shadows; that means if you use built-in [Transparent](shader-transparentfamily.html) or Particle shaders then you'll get no shadows. In most cases it's possible to [Transparent Cutout](shader-transparentcutoutfamily.html) shaders (for objects like fences, vegetation etc.). If you use custom written [Geometry render queue](shaders]],theyhavetobepixel-litanduse[[sl-subshadertags.html). Objects using <span class=component>VertexLit</span> shaders do not receive shadows either (but can cast shadows just fine).

Finally, in [Forward rendering path](rendertech-forwardrendering.html), only the brightest directional light can cast shadows. If you want to have many shadow casting lights, you need to use [Deferred Lighting](rendertech-deferredlighting.html) rendering path.
