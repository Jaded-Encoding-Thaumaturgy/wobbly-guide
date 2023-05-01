# Handling Pattern Guessing Failures

After pattern guessing and fixing framerates,
there may still be pattern guessing failures.

Useful keybinds for this section:

| Key                       | Action                                   |
| ------------------------- | ---------------------------------------- |
| Left Arrow                | Jump 1 frame back |
| Right Arrow               | Jump 1 frame forward |
| S                         | Cycle the current frame's match |
| D                         | Toggle decimation for the current frame |
| Ctrl + F                  | Replace current frame with previous frame (freezeframe) |
| Shift + F                 | Replace current frame with next frame (freezeframe) |


## Leftover Combing

Pattern guessing may sometimes leave you with random combed frames
that could not be matched automatically.
Open the "Combed frames" menu.

![A list of all the combed frames found](imgs/combed_frames.png)

Before you do anything,
click "Refresh".
This will perform another search through the clip
to find any remaining combed frames.
This may take a couple of minutes to finish.

![Finding combed frames...](imgs/finding_combs.png)

You can now double-click on all the found combed frames,
or jump to the next combed frame using .
For any combed frame,
you can press `S` to cycle through fieldhints.
If every cycle returns a combed frames,
consider adjusting the decimated frame
(using `D` to swap between decimated and not,
making sure you don't ruin the framerates you just fixed),
or pulling it down in your filterchain later.

Another thing to take into account is that this will also find telecined fades.
You typically do not want to perform fieldmatching on the fade itself,
but just the underlying animation.
If the caught combed frame is caused by the fade,
ignore it
and process it with a filter meant to deal with those
in your filterchain later.


## Freezeframing

If you find scenes of a duplicated clip
(that was not decimated due to being animated on twos/threes/fours)
that has very heavy compression artifacting,
it might be worth it to freezeframe it with either the next frame
(`Shift + F`)
or the previous frame
(`Ctrl + F`).
You can adjust these later in the "Frozen frames" window.
This usually won't be applicable or worth it
unless you're dealing with *very* starved video
and heavy MPEG2 blocking.


## Crossfades

When dealing with fades to and from scenes,
you'll want to put the scene change somewhere in the middle.
The first frame before a fade in is usually the best,
unless it fades in from a solid colour with a clear scenechange.
To deal with crossfades
(that is, two scenes that fade into each other
without a solid color inbetween)
where the pattern differs between scenes,
you can try creating a new section
that captures just the fade.
Wobbly may be able to accurately decimate that for you.
If the pattern remains the same,
there is no reason to do this.
