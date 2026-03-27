---
title: "Mixing with reverb"
---

> Download the project files [here](https://dakotastateuniversity-my.sharepoint.com/:f:/g/personal/tate_carson_dsu_edu/EkKJ0ZNmVo9FmSzc656-tMEB1sk-aWTBacwhKNzcxwMyFA?e=PK9yfP).

What is reverb used for? It can enhance these elements:

- **Blend** - Glue together tracks that were recorded in different spaces. Applying the same reverb to multiple instruments places them in a shared acoustic environment so they sound like they belong together.
- **Size** - Make a sound feel like it's in a specific space. A short reverb puts a close-miked vocal in a small room; a long reverb places it in a cathedral. This controls perceived depth and distance in the mix.
- **Tone** - Shape the brightness or darkness of a sound. A bright reverb with a short pre-delay adds air and presence to a vocal, while a dark, dampened reverb can warm up a harsh guitar and push it further back.
- **Sustain** - Extend the tail of short, percussive sounds. Adding reverb to a snare hit or a plucked string lets it ring out and fill space rather than cutting off abruptly.
- **Spread** - Widen a mono or narrow source across the stereo field. A stereo reverb on a center-panned vocal or lead instrument makes it feel bigger without changing its pan position.

> Examples from [Chapter 16: Mixing With Reverb](https://cambridge-mt.com/ms/ch16/)

---

Now we mostly use plugins for reverb, but reverb predates digital effects. Some of the ways engineers used to generate reverb were: chambers, plates, and springs.

### Inside the reverb chambers at Capricorn Sound Studios

<iframe width="560" height="315" src="https://www.youtube.com/embed/Am0ELIQcCgQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Spring reverb

<iframe width="560" height="315" src="https://www.youtube.com/embed/tU7U-U-n4EQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Plate reverb

<iframe width="560" height="315" src="https://www.youtube.com/embed/Y58nroQ0DMw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Reaper stock plugins:

- ReaVerb
- ReaVerbate

See the [ReaEffects guide](https://www.reaper.fm/guides/REAPEREffectsGuide2021.pdf) for more details.

## ReaVerbate

Let's first learn how to use ReaVerbate on single instruments. Then we'll use it to enhance the elements mentioned above. ReaVerbate is the standard reverb plugin for Reaper. Add it to the guitar track in your project.

Parameter descriptions (from the ReaEffects guide):

**Wet**
Controls how much processed (wet) signal you hear.

**Dry**
Controls how much unprocessed (dry) signal you hear.

**Room size**
Sets the size of the room you are simulating.

**Dampening**
Simulates absorption from soft surfaces like curtains and carpet, darkening the reverb.

**Stereo Width**
Narrows or widens the stereo field of the reverb.

**Initial Delay**
Adds a delay of a specified number of milliseconds before the reverb starts. Higher settings create a feeling of more space.

**Lowpass**
Cuts reverb above this frequency.

**Highpass**
Cuts reverb below this frequency. Reverb applies only to frequencies between the highpass and lowpass settings.

### Reverb on one instrument

With the room size at 100, turn the dampening up and down. You should hear that a low level of dampening creates a bright reverb, and more dampening darkens the reverb. To further color the sound, use the high and low pass filters.

### Reverb on a send

Because we often want the same reverb on multiple instruments, we can use a send in Reaper, which is just another track.

Create a new track next to the drums and call it "Reverb." To route your drums into this send:

1. Select all of the drum tracks.
2. Hold shift and drag them onto the Reverb track.

You should now see in the routing section that all of your drums are going through the Reverb track.

Now add ReaVerbate to this reverb send track. Because this is a send track we control the amount of reverb by our send level. So, set the wet mix to 0 dB and the dry mix to -inf dB.

Open the routing for the reverb send and turn all of the send levels to -inf dB. We'll bring up the send levels one track at a time. Increase the level of the snare first, then add some to the overheads.

> - Try to make your own presets for the Guitar and Vocal tracks.
> - Now try this whole process on your drum editing project from earlier in the semester.

## ReaVerb

We can also use ReaVerb, a plugin that allows you to customize your reverb. It can do convolution, but also much more. It contains the following modules: Echo generator, reverb generator, convolution reverb file, high/low pass filters, normalization, reverse, time/gain/stretch. Let's use it to create a sound effect from a cat meowing.

View the [ReaEffects guide](https://user.cockos.com/~glazfolk/ReaEffectsGuide.pdf) for details on each parameter. We'll look at each module one at a time.

- Echo generator - creates echoes or delays of the signal
- File - add a sound file to convolve the signal with
  - Go [here](https://www.voxengo.com/impulses/) to download some impulse files to play around with.
  - If the reverb is very loud, apply a -18 dB gain to the file.
- Reverse
- Time/Gain/Stretch - combined with reverse, creates a riser effect


### Quick in-class exercise: ReaVerb vs. ReaVerbate

Places to look for impulse responses:

- [OpenAIR Library](https://openairlib.net/) - a very good source for real acoustic spaces.
- [EchoThief](https://www.echothief.com/downloads/) - lots of unusual and characterful spaces.
- [Voxengo Impulses](https://www.voxengo.com/impulses/) - a quick set of free IRs that works well for practice.

1. Find three contrasting impulse responses to try in ReaVerb. Choose clearly different spaces or textures, such as a small room, a plate, a spring, or a long hall.
2. Load each impulse response into ReaVerb on the same track or bus and listen to how the sound changes.
3. Pick one impulse response to focus on. 
4. Replace ReaVerb with ReaVerbate on the same source.
5. Try to mimic the character of that impulse response using only ReaVerbate's controls: room size, dampening, initial delay, stereo width, and the highpass/lowpass filters.
6. Switch back and forth between the ReaVerb version and the ReaVerbate version until you get as close as you can.
7. If we have more time, try to mimic the other two impulse responses as well.
8. Be ready to share which impulse response you chose and which parts were easiest or hardest to imitate with an algorithmic reverb.
