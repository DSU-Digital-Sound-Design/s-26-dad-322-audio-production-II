---
title: "EQ Lab"
---

## Due

Due **Wednesday, March 11, 2026 at 2:00 pm** (submit to D2L).

## Goal

Practice using EQ (and basic gating) to reduce spill/leakage, remove noise, and shape timbre while keeping sources sounding natural.

## What to Turn In

- A rendered stereo mixdown for each section below (mp3 or wav is fine).
- Your Reaper project file(s) used to create those renders.
- Short notes (a few bullets per section) listing the main EQ moves you made (filters, rough frequencies, and why).

## Downloads

Download the following source projects/files for the EQ lab.

## Jesper Buhl Trio - What is this thing called love

[Jesper Buhl Trio](https://mtkdata.cambridgemusictechnology.co.uk/MTK002/MR0804_JesperBuhlTrio.zip)

- Create a balanced mix (levels and panning first).
- Use **ReaGate** to reduce spill on each microphone (keep it subtle and avoid obvious pumping/chatter).
- **Snare:** Use peaking filters to get the snare tone you want. Then try to reduce leakage from other instruments without ruining that snare tone. Prioritize “natural” over “perfect isolation.”
- **Bass:** Reduce leakage with a high-cut or HF-shelf. Use peaking and/or notch filters to tame unpleasant resonances and add definition.

## Bobby Nobody - Stitch up

[Bobby Nobody](https://mtkdata.cambridgemusictechnology.co.uk/MTK003/MR0911_BobbyNobody.zip)

- Create a balanced mix (levels and panning first).
- Use **ReaGate** to reduce spill on each microphone (again: subtle is better than artifacts).
- **Bass cab:** Attenuate unpleasant resonances and adjust the overall tone so it fits with the band. Use primarily peaking and notch filters.

## Audio processing pack

[link](http://ocw.mit.edu/ans7870/21m/21m.380/S12/audioProcReport01.zip)

- `femaleVoice02.aif`: Identify the low-frequency background rumble (use good headphones or monitors). Remove it with a low-cut filter *without* noticeably changing the vocal tone.
  - Alternative: remove it with **ReaFIR** (FFT mode).
- `kick01.aif`: Reduce leakage and improve kick definition without creating harsh resonances. Use a high-cut or HF-shelf plus peaking/notch filters as needed.

## Guitar Hum

[Guitar Hum](https://audio.cambridge-mt.com/MSFTSS/Ch11/MS1116_GuitarHum01_Raw.wav)

Remove the AC hum on the guitar. The best approach is usually a series of very narrow notch filters at the power-line fundamental and its harmonics:

- **60 Hz** (most of the US) or **50 Hz** (many other countries)
- Then 120/180/240... (or 100/150/200...) as needed

Keep the notches as narrow as possible, and use only as many as you need to make the noise unobtrusive.
