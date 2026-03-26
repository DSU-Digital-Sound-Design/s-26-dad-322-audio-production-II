---
title: "Mixing with Reverb"
---

Let's go back to our uses for reverb:

- Blend
- Size
- Tone
- Sustain
- Spread

Finding good settings takes trial and error, so we'll install many free reverb plugins and try them on different musical elements. The Reaper reverbs are good starts, but different algorithms suit different uses, so more options help.

Download and install the following reverb plugins:

- Basics:
  - [OrilRiver](https://www.kvraudio.com/product/orilriver-by-denis-tihanov)
  - [Sanford](https://www.lesliesanford.com/vst/plugins/) - PC only
  - [Ambience](http://magnus.smartelectronix.com/#Ambience) - may not load on all systems
- Creative plugins for tone and sustain
  - [PSP PianoVerb](https://www.pspaudioware.com/products/psp-pianoverb)
  - [Valhalla Supermassive](https://valhalladsp.com/shop/reverb/valhalla-supermassive/)
  - [KR-Reverb FS R1.5.0](https://www.kresearch.com/Products/Details/17)
    - The UI on this looks strange but it sounds really great. Notice the unique "listener position" setting. You can also set the size of the early reflections and tail separately.
  - [Dragonfly Reverb](https://michaelwillis.github.io/dragonfly-reverb/) - [Manual](https://michaelwillis.github.io/dragonfly-reverb/manuals.html)
  - [Riviera: Hyper-room reverb](https://nuspaceaudio.com/2017/02/07/riviera-fast-hybrid-reverb-plugin-for-modeling-high-dimensional-spaces/)
  - [TAL Reverb 2 + 3](https://tal-software.com/products/tal-reverb)
  - [TAL Reverb 4](https://tal-software.com/products/tal-reverb-4)
  - [Protoverb](https://u-he.com/products/protoverb/)
  - [Xhip Reverb](http://xhip.net/effects/?p=Reverb) - GUI may not load on all systems
- Convolution
  - [MConvolutionEZ](https://www.meldaproduction.com/MConvolutionEZ)
- New to this course:
  - [TENS jr.](https://www.audiopluginsforfree.com/tens-jr/) - great sounding spring 
  - [Flex Reverb](https://www.audiopluginsforfree.com/flex-reverb/) - flat-sounding, but clean interface
  - [Reverb | Airwindows](https://www.airwindows.com/category/reverb/)
  - [FogPad - Reverb plugin](https://www.igorski.nl/download/fogpad)

Let's go to [Mike's page](https://cambridge-mt.com/ms/ch16/) for some advice on choosing reverbs and working with them.

## Size

Follow Mike's method for finding a reverb preset for blend/size. He plays [this drum sound](https://audio.cambridge-mt.com/MSFTSS/Ch16/MS1601_Preset0Dry.wav) through different reverbs to compare them. Create a new project with this sample, then create a reverb bus and send the drum through it.

Find an instrument that could have a larger size in the mix. Use the suggestions from the book to find a good preset for the instrument.

> The biggest difference between reverbs designed for blend and size is that where the former is best provided by the earlier reverb reflections, the latter is best created by focusing the effect sound on the remainder of the reverb tail.

I'll try OrilRiver for this. If you could get Sanford or Ambience to work those are also good options. Let's check out the [manual](orilriver-manual.pdf). Let's explore the settings of this reverb.

Try turning off the reverb tail to hear only the early reflections. Adjust the room size parameter to hear how they change. Then do the reverse: turn off early reflections and listen to the tail alone.

The room size parameter mostly affects the early reflections.

Try to mimic the first 4 presets that Mike lists on [his site](https://cambridge-mt.com/ms/ch16/).

> - Beware of unnatural-sounding presets, as these will have trouble creating the sound of a larger space convincingly. CPU-light plug-ins will typically sound less natural than more computationally hungry algorithms.
> - Feel free to ignore the preset names with impunity—the main goal is to try to imagine the space implied by each preset and decide whether it’s the right kind of space for your mix to exist within.
> - Don’t be too concerned about tonal imbalances as long as there aren’t nasty metallic resonances.
> - Check that the stereo picture is fairly evenly spread, and assess the mono compatibility.
> - Don’t hurry the selection process, and make sure you ratify your choice properly with your different monitoring systems.
> - When you’ve got a promising patch, mute it, recalibrate your ears to the mix as is, and then fade it up to confirm that it’s actually what you’re looking for.

## Blend

Use the most natural-sounding reverbs for blending. Pay special attention to predelay settings. Predelay indicates the size of the room — in a large room, predelay is longer because reflections take longer to return to the listener. Generally use a predelay between 10-20ms.

Try to blend like elements. Drums should blend, vocals and background vocals, horn sections.

When working with multiple tracks of the same type, you may want to control the send amounts together. Here's one method:

> 1. Create a new track called `Drum Verb`.
> 2. Move your FX to that track by clicking the FX icon and dragging with `option` held down.
> 3. Rename your original reverb track to `Drum Verb Send`.
> 4. Remove `Drum Verb Send` from the master parent send: click routing and uncheck `Parent send`.
> 5. Route `Drum Verb Send` to `Drum Verb`.
>
> You now have a master control over the send levels for all drum tracks, making it easy to automate reverb as a group.

## Tone and sustain

Unlike blend and size reverbs, tone and sustain reverbs can sound unnatural. The goal isn't to simulate a space but to reshape the sound's character. Spend time exploring your reverbs to find ones that produce distinctive textures.
