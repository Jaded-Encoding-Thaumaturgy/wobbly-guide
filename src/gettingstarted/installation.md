# Installation

To install Wobbly, you must first navigate to its [download page][wobbly_release].
The recommended version as of writing this guide is the [Setsugennoao fork, release v6-R2][recommended_version].

You can get the latest version by going to the *Actions* tab,
clicking on the latest workflow,
and clicking on the *Wobbly-win64* link under *Artifacts*.
It should start downloading Wobbly now.

![A Wobbly artifact](imgs/wobbly_artifact.png)

To continue, you must now unpack this zip file.
Make sure you unpack it in a place you're sure it won't be moved from in the future!
The easiest place to put it is in your Documents directory.

## Dependencies

Wobbly has the following dependencies:

* [d2vsource](https://github.com/dwbuiten/d2vsource) (optional, input dependent)
* [DGDecNV](https://www.rationalqm.us/dgdecnv/dgdecnv.html) (optional, input dependent)
* [DMetrics](https://github.com/vapoursynth/dmetrics)
* [FieldHint](https://github.com/dubhater/vapoursynth-fieldhint)
* [L-SMASH-Works](https://github.com/AkarinVS/L-SMASH-Works) (optional, input dependent, through Akarin)
* [SCXVID](https://github.com/dubhater/vapoursynth-scxvid)
* [TDeintMod](https://github.com/HomeOfVapourSynthEvolution/VapourSynth-TDeintMod)
* [vivtc](https://github.com/vapoursynth/vivtc)

You can verify it can find the plugins by opening Wobbly,
hovering over the "Tools" dropdown menu at the top of the window,
and clicking on "Check plugins".

![Checking installed plugins](imgs/check_plugins.png)

This will open up a window displaying the plugins it was able to find.

![Installed plugins](imgs/installed_plugins.png)


[//]: <> (urls)
[wobbly_release]: https://github.com/Setsugennoao/Wobbly/releases
[recommended_version]: https://github.com/Setsugennoao/Wobbly/actions
