# Limitations

Before you get started,
it's important to be aware of the limitations that come with Wobbly.
No software is perfect,
and this holds true for Wobbly as well.


## 5-Frame Cycles Only

Wobbly is limited to 5-frame cycles.
This means it can only ever be used for NTSC content
(such as Japanese or North-Americans DVDs,
see [this wikipedia page][PAL_NTSC] for more information),
and will not work on PAL/SECAM video.

This also includes variable telecine cycles.
Wobbly always assumes a clean 3:2 Pulldown algorithm
was applied to the input clip,
and no support is currently given for other patterns.

## Deinterlaced Footage

Wobbly has no support for footage that was deinterlaced
or pre-fieldmatched.
Deinterlacing comes in many shapes and sizes,
the most common of which is through filters
such as YADIF (found in FFMpeg).
These are destructive by nature
and will not give Wobbly anything to work with.
Another common example of deinterlaced footage
is footage with blended fields
(which often matches the original telecining pattern,
such as AABBA).

![An example of blended footage (Fate/EXTRA Extella OP1)](imgs/blended_fields.png)

Similarly,
content that has its fields already matched
and only requires decimation are not currently supported in Wobbly.
It relies on knowing the fieldmatches
to determine how a clip should be decimated.
It simply does not know what to do with progressive content.

## "True" VFR

Wobbly does not currently support *true* VFR.
Decimation is strictly based on the telecine cycle,
meaning that VFR ranges get rounded.
This is a side-effect of Wobbly only supporting a very limited number of framerates
(6, 12, 18, 24, 30).

Similarly,
Wobbly does not currently allow you to easily output 59.94 frame/s video.
This can become an issue when you must deinterlace a scene
and want to make use of the timecodes provided by Wobbly.


## Decimation Breaks

This is a regression from YATTA.

Due to the way footage was commonly edited
during the early digital era,
a lot of editing was done on telecined footage.
This means you may get splices that results in extra frames being left in,
ruining the decimation cycle.
Wobbly will simply set it to a wrong framerate,
whereas YATTA would automatically determine this was the case
and add a decimation by itself.
We cover how to do this manually in the *[Fixing the Framerate][framerates_guide]* section,
but it's something that should honestly be done automatically.


[//]: <> (urls)
[PAL_NTSC]: https://en.wikipedia.org/wiki/DVD_region_code#PAL/SECAM_vs._NTSC
[framerates_guide]: //
