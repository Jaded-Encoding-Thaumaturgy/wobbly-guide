# Making Use of the Wobbly Output

There are two straightforward ways to make use of the clip you've just fixed up in Wobbly.

## From Wobbly Itself

Within Wobbly's "Project" dropdown menu,
you can save a script.
This will output a "vpy" file
next to the Wobbly JSON file.

![Dropdown Options](imgs/save_script.png)

![Generated Script](imgs/generated_script.png)

You can simply stick the contents of this script into your own script and work from there.

Wobbly can also output a timecode file.
This should be muxed into the final container alongside your video
to make sure it properly displays VFR content.
If the end result is a *Constant Framerate*,
you can skip that so long as you mark the framerate correctly during encoding.

## Using an External Tool

TODO: I would describe vswobbly here... IF I'D FINISHED WRITING IT!
