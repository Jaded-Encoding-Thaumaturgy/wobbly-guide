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

Make sure you set the Field Based property to "Progressive" after you've imported the script!
This can be done using either of these functions:

### Using stdlib

```py
src = src.std.SetFieldBased(0)
```

### Using vstools

```py
from vstools import FieldBased

src = FieldBased.PROGRESSIVE.apply(src)
```

## Using vs-wobbly

TODO

## Timecodes

Wobbly can also output a timecode file.
This should be muxed into the final container alongside your video
to make sure it properly displays VFR content.
If the end result is a *Constant Framerate*,
you can skip that so long as you mark the framerate correctly during encoding.
