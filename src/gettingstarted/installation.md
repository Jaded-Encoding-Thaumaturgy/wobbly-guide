# Installation

We recommend downloading Wobbly from the [JET fork][wobbly_release].

To continue, you must unpack the zip file.
Make sure you unpack it in a place where you're sure it won't be moved from in the future!
An easy place to put it is in your Documents directory.

## Downloading a pre-release version

If the most recent release is not up to date with the master branch,
then you might want to consider downloading the [latest master build][actions_page].
If the build has not expired yet, it will start downloading the latest snapshot.

![A Wobbly artifact](imgs/wobbly_artifact.png)

## Dependencies

Wobbly has the following dependencies:

* [BestSource](https://github.com/vapoursynth/bestsource) (optional, input dependent)
* [d2vsource](https://github.com/dwbuiten/d2vsource) (optional, input dependent)
* [DGDecNV](https://www.rationalqm.us/dgdecnv/dgdecnv.html) (optional, input dependent)
* [DMetrics](https://github.com/vapoursynth/dmetrics)
* [FieldHint](https://github.com/dubhater/vapoursynth-fieldhint)
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
[wobbly_release]: https://github.com/Jaded-Encoding-Thaumaturgy/Wobbly/releases
[actions_page]: [https://github.com/Jaded-Encoding-Thaumaturgy/Wobbly/actions](https://nightly.link/Jaded-Encoding-Thaumaturgy/Wobbly/workflows/windows/master/Wobbly-win64.zip)
