Audio Listener
==============


The <span class=keyword>Audio Listener</span> acts as a microphone-like device. It receives input from any given [Audio Source](class-audiosource.html) in the scene and plays sounds through the computer speakers. For most applications it makes the most sense to attach the listener to the Main [Camera](class-camera.html). If an audio listener is within the boundaries of a [Reverb Zone](class-audioreverbzone.html) reverberation is applied to all audible sounds in the scene. (PRO only) Furthermore, [Audio Effects](class-audioeffect.html) can be applied to the listener and it will be applied to all audible sounds in the scene.   

![](http://docwiki.hq.unity3d.com/uploads/Main/audio_listener_inspector.png)  
_The Audio Listener, attached to the Main Camera_


Properties
----------


The Audio Listener has no properties.  It simply must be added to work.  It is always added to the Main Camera by default.


Details
-------


The Audio Listener works in conjunction with [Audio Sources](class-audiosource.html), allowing you to create the aural experience for your games.  When the Audio Listener is attached to a <span class=keyword>GameObject</span> in your scene, any Sources that are close enough to the Listener will be picked up and output to the computer's speakers.  Each scene can only have 1 Audio Listener to work properly.

If the Sources are 3D (see import settings in [Audio Clip](class-audioclip.html)), the Listener will emulate position, velocity and orientation of the sound in the 3D world (You can tweak attenuation and 3D/2D behavior in great detail in [Audio Source](class-audiosource.html)) .  2D will ignore any 3D processing. For example, if your character walks off a street into a night club, the night club's music should probably be 2D, while the individual voices of characters in the club should be mono with their realistic positioning being handled by Unity.

You should attach the Audio Listener to either the Main Camera or to the GameObject that represents the player. Try both to find what suits your game best.

Hints
-----


* Each scene can only have one Audio Listener.
* You access the project-wide audio settings using the [Audio Manager](class-audiomanager.html), found in the <span class=menu>Edit->Project Settings->Audio</span> menu.
* View the [Audio Clip](class-audioclip.html) Component page for more information about Mono vs Stereo sounds.

