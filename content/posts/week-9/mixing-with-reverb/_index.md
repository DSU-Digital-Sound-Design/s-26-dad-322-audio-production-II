---
title: "Mixing with reverb"
---

> Download the project files [here](https://dakotastateuniversity-my.sharepoint.com/:f:/g/personal/tate_carson_dsu_edu/EkKJ0ZNmVo9FmSzc656-tMEB1sk-aWTBacwhKNzcxwMyFA?e=PK9yfP).

What is reverb used for? It can enhance these elements:

- Blend
- Size
- Tone
- Sustain
- Spread

> Examples from [Chapter 16: Mixing With Reverb](https://cambridge-mt.com/ms/ch16/)

---

Now we mostly use plugins for reverb, but reverb has a history before digital effects. Some of the ways engineers used to generate reverb were: chambers, plates and springs.

### Inside the reverb chambers at Capricorn Sound Studios

<iframe width="560" height="315" src="https://www.youtube.com/embed/Am0ELIQcCgQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Spring reverb

<iframe width="560" height="315" src="https://www.youtube.com/embed/tU7U-U-n4EQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Plate reverb

<iframe width="560" height="315" src="https://www.youtube.com/embed/Y58nroQ0DMw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Reaper stock plugins:

- ReaVerb
- ReaVerberate

See the [ReaEffects guide](https://www.reaper.fm/guides/REAPEREffectsGuide2021.pdf) for more details.

## ReaVerbate

Let's first learn how to use ReaVerbate on single instruments. Then we'll use it to enhance the elements mentioned above. ReaVerbate is the standard reverb plugin for Reaper. Add it to the guitar track in your project.

Parameter descriptions (from the ReaEffects guide):

**Wet**
Determines the amount of the processed (wet) signal mixed into the outgoing audio stream.

**Dry**
Determines the amount of the unprocessed (dry) signal mixed into the outgoing audio stream.

**Room size**
Specifies the size of the room whose natural reverberation you are aiming to imitate.

**Dampening**
Moderates the reverb effect to allow for the fact of items such as curtains and carpet that might be present in the room.

**Stereo Width**
This control can be used to reduce the stereo field of the reverb effect.

**Initial Delay**
Allows for a delay ODF a specified number of milliseconds before the reverb is produced. Higher settings can sometimes create a feeling of more space.

**Lowpass**
Used to ensure that the reverb is not applied to higher frequencies (above the lowpass setting).

**Highpass**
Used to ensure that the reverb is not applied to lower frequencies (below the highpass setting). Reverb will be applied to all frequencies in the range between the highpass and lowpass filter settings.

### Reverb on one instrument

With the room size at 100 turn the dampening up and down. You should hear that a low level of dampening creates a bright reverb, and more dampening darkens the reverb. To further color the sound you can use the high and low pass filters.

### Reverb on a send

Because of our uses of reverb that we stated earlier, we often want to apply the same reverb sound to multiple instruments. You can do this in Reaper with a send, which is just another track.

Create a new track by the drums and call it reverb. To route your drums into this send select all of the drums then click shift and then drop onto the Reverb track. You can now see in the routing section that all of your drums are now going through the Reverb track.

Now add ReaVerbate to this reverb send track. Because this is a send track we control the amount of reverb by our send level. So, set the wet mix to 0 dB and the dry mix to -inf dB.

Open the routing for the reverb send and turn all of the send levels to -inf dB. We'll bring up the send levels one track at a time. Increase the level of the snare first, then add some to the overheads.

> - Try and make your own presets for the Guitar and Vocal tracks.
> - Now try this whole process on your drum editing project from earlier in the semester.

## ReaVerb

We can also use ReaVerb, a plugin that allows you to customize your reverb. It can do convolution, but also much more. It contains the following modules: Echo generator, reverb generator, convolution reverb file, high/low pass filters, normalization, reverse, time/gain/stretch. Let's use it to create a sound effect from a cat meowing.

Again, view the [ReaEffects guide](https://user.cockos.com/~glazfolk/ReaEffectsGuide.pdf) here for details on what all of the parameters do. We'll look at each module one at a time.

- Echo generator - this makes a lot of echos or delays of the signal
- File - add a sound file to convolve the signal with
  - Go [here](https://www.voxengo.com/impulses/) to download some impulse files to play around with.
  - If the reverb is very loud, apply a -18 dB gain to the file.
- Reverse
- Time/Gain/Stretch - can create a really cool riser effect with this and reverse

### Other good reverb plugins:

- [MCharmVerb](https://www.meldaproduction.com/MCharmVerb)
- [MConvolutionEZ](https://www.meldaproduction.com/MConvolutionEZ)
- [PSP PianoVerb](https://www.pspaudioware.com/products/psp-pianoverb)
- [PSP Chamber](https://www.pspaudioware.com/products/psp-chamber)
- [Valhalla Supermassive](https://valhalladsp.com/shop/reverb/valhalla-supermassive/)
