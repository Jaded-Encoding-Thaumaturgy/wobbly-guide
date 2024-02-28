# Installation

We recommend downloading Wobbly from the [Setsugennoao fork][wobbly_release].

To continue, you must unpack the zip file.
Make sure you unpack it in a place where you're sure it won't be moved from in the future!
An easy place to put it is in your Documents directory.

## Downloading a pre-release version

If the most recent release is not up to date with the master branch,
then you might want to consider downloading from the [actions page][actions_page].
You can get the latest snapshot by going to the *Actions* tab,
clicking on the latest workflow,
and then click on the *Wobbly-win64* link under *Artifacts*.
If the artifacts link has not expired yet, it will start downloading the latest snapshot.

![A Wobbly artifact](imgs/wobbly_artifact.png)

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
[actions_page]: https://github.com/Setsugennoao/Wobbly/actions
