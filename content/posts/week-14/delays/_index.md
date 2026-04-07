---
title: "Mixing with Delays"
---

> First, listen to [Mike Senior's delay examples](https://cambridge-mt.com/ms/ch17/).

## Delays in Reaper

Delay is a close cousin of reverb. Reverb creates many repeats packed tightly together; delay creates repeats spaced farther apart.

Open the Reaper starter project [here](https://dakotastateuniversity-my.sharepoint.com/:f:/g/personal/tate_carson_dsu_edu/Eu21oE1GkClLoqCG_joBRawB_Z6nDF-dYYNT-rOoMzAStg?e=epotLO). Add `ReaDelay` to the `Flute` track. By default, delay time uses `Length (musical)`. Adjust it to taste, preferably to a whole number. If the repeats feel out of time, set the correct project tempo.

Next, raise `Feedback` to hear longer repeat trails. Then adjust the filter section to color the repeats.

Create a stereo multi-tap delay. Pan the first tap left. Create a second tap and pan it right. Build complex rhythms by changing the tap times.

You can also set delay time in milliseconds instead of musical values. Around `100 ms` creates a slapback echo.

> Run your own delay experiments on the spoken-word vocal. Build a texture with multiple taps, then try chaining several `ReaDelay` instances in series for more complex effects.

## Dynamic delay

This technique is similar to the dynamic reverb method from earlier weeks. The delay comes in and out based on signal dynamics.

Create a delay send track and route your vocal to it. Add `ReaDelay` to the `Delay` track. Turn off the dry signal because the dry vocal already comes from the source track.

Set `Length (musical)` to `2`, increase feedback, and filter the repeats to thin them out.

Automate the delay using the same method from the dynamic reverb lesson.

Now try the same approach with a compressor after the delay. Drag the vocal track routing icon onto the compressor so track channels `1/2` feed auxiliary channels `3/4`. Set detector input to `Auxiliary Inputs`. Set attack and release to `0`, and set ratio to `inf`. Then lower threshold until you hear mostly delayed signal when the vocal pauses. Finally, lengthen release for a subtler effect.

> Create your own dynamic delay on a synth part with spaces in it. Program the delay to turn on only when the synth pauses. Use any synth; if you need one, try [Vital Synth](https://vital.audio/).

## Automated delay

This is similar to dynamic delay, but the effect turns on only for selected notes or syllables. You get tighter control by automating delay mute. Set up a delay send track as before and route the vocal to it.

Open the vocal track envelopes window. In `Send Envelopes`, select `Delay Send Mute`. Draw the envelope so mute is off only for the word "then." Listen closely to the rhythm of both repeats and match their timing.

> You can also create a delay throw by automating delay volume instead of mute. Recreate the same effect with volume automation. This gives finer control over the sound. We will go deeper on automation in the next lesson.

## Coloristic and more extreme delays

If time allows, explore these delay effects.

- [Chow Matrix](https://chowdsp.com/products.html)
- [Valhalla Freq Echo](https://valhalladsp.com/shop/delay/valhalla-freq-echo/)
- [Full Bucket Brigade Delay](https://www.fullbucket.de/music/fbdelay.html)
