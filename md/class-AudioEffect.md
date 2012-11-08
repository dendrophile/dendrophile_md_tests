Audio Filters (PRO only)
========================


[AudioSources](class-AudioSource.html) and the [AudioListener](class-AudioListener.html) can have filter components applied, by adding the filter components to the same GameObject the AudioSource or AudioListener is on. Filter effects are serialized in the component order as seen here:

![](http://docwiki.hq.unity3d.com/uploads/Main/FilterGraph1.png)  

Enabling/Disabling a filter component will _bypass_ the filter. Though highly optimized, some filters are still CPU intensive. Audio CPU usage can monitored in the [profiler](Profiler#Audio.html) under the Audio Tab.


See these pages for more information on each filter type:
* [Low Pass Filter](class-AudioLowPassFilter.html)
* [High Pass Filter](class-AudioHighPassFilter.html)
* [Echo Filter](class-AudioEchoFilter.html)
* [Distortion Filter](class-AudioDistorionFilter.html)
* [Reverb Filter](class-AudioReverbFilter.html)
* [Chorus Filter](class-AudioChorusFilter.html)

