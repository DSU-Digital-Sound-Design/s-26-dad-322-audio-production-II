---
title: "Compression Lab"
---

### Overview

This lab introduces the practical use of compression in audio mixing. You’ll install a few free compressors, then practice controlling dynamics on drums and vocals so the mix feels more consistent, punchy, and “glued together” without getting louder just because it’s compressed.

### Objectives

- Explain what a compressor is doing (what changes when you move threshold, ratio, attack, release, and output gain).
- Hear (and measure) gain reduction and describe what it sounds like on drums vs. vocals.
- Apply compression to individual tracks and to a drum bus while keeping levels matched for fair A/B comparisons.

### Required Materials

- The Hurray For the Riff Raff drum editing project (or a similar multi-track drum recording).
- A vocal sample or vocal session to apply compression to.

### Step 1: Preparation

#### Download and Install Compressors

1. **MCompressor**: Visit [MeldaProduction](https://www.meldaproduction.com/MCompressor) to download and install MCompressor.
2. **TDR Kotelnikov**: Download TDR Kotelnikov from [Tokyo Dawn Records](https://www.tokyodawn.net/tdr-kotelnikov/).
3. **Tukan – Compressor 2 (REAPER)**: Install via ReaPack by following this guide: [Free REAPER Plugins: Tukan](https://untidymusic.com/free-reaper-plugins/free-reaper-plugins-tukan). After you add/sync the Tukan repo in ReaPack, search for **Compressor 2** in **Extensions → ReaPack → Browse packages**, install it, then find it in the FX browser under **JS/JSFX** (search “Tukan”).


#### Explore Compressor Settings

- Spend 2–3 minutes with each compressor and locate these controls (names vary by plugin):
  - **Threshold** (when compression starts)
  - **Ratio** (how much it compresses after threshold)
  - **Attack / Release** (how fast it reacts and recovers)
  - **Makeup / Output** (how you level-match after compression)
  - **Gain reduction meter** (how many dB the compressor is turning down)
- If a plugin has **auto-makeup**, turn it **off** for this lab unless instructed otherwise. Auto-makeup can make “compressed” sound seem “better” simply because it’s louder.

#### Quick Listening Rule (Important)

When you compare “before vs. after,” keep the loudness as close as possible. If the compressed version is louder, it will almost always *feel* better even if the settings are worse. Use the plugin’s output gain (or the track fader) to match levels when A/B-ing.

### Step 2: Applying Compression to Drums

#### Compress the Kick Drum

1. Open the Hurray For the Riff Raff drum editing project.
2. Insert ReaComp (or your chosen compressor) on the kick drum track.
3. Start with a **ratio of 4:1**.
4. Lower the **threshold** until you see around **3–6 dB** of gain reduction on the loud hits.
5. Start with **attack 10–30 ms** (to keep some punch) and **release 50–150 ms** (so it recovers between hits). Adjust by ear.
6. Use **output/makeup** to level-match the compressed signal to the bypassed signal.

What to listen for:
- More consistent kick level from hit to hit
- More “body”/sustain (if release is longer)
- Less “click”/transient (if attack is too fast)

#### Apply to Other Drums

- Repeat the process for other close drum mics (snare, toms, etc.). Use the same workflow:
  1. Set a ratio.
  2. Set threshold to hit a gain-reduction target.
  3. Adjust attack/release to shape the transient vs. sustain.
  4. Level-match output, then A/B.
- For hi-hats/cymbals, start gently (or skip compression). It’s easy to make cymbals sound harsh or “sucked down.”

To hear the cumulative effect, periodically **bypass compressors** and listen to the full kit:
- Bypass per-track by toggling the track’s **FX** button (or bypassing the compressor inside the FX chain).
- When you A/B, keep levels matched.

#### Compress Room Microphones

1. Apply a compressor to the room microphone tracks. Consider using the 1175 Compressor from Reaper or one of the plugins you downloaded.
2. Start with a **ratio of 4:1** and lower the threshold until you see **6–12 dB** of gain reduction (room mics can handle more compression).
3. Try a **faster attack** and **medium release** to bring up room tone and excitement.
4. Manually adjust **output gain** so the room track isn’t “better” just because it’s louder.

#### Group Compression

1. Group all drum tracks into a folder.
2. Apply a compressor to the **drum folder/bus**.
3. Start subtle: **2:1**, threshold for **1–3 dB** gain reduction on the loudest sections, then level-match.
4. Then experiment: push it harder and notice when the kit starts to pump, lose punch, or feel smaller.

What to listen for on the drum bus:
- “Glue” (kit feels more like one instrument)
- Pumping/breathing (sometimes cool, sometimes distracting)
- Transient loss (attack too fast) vs. unevenness (attack too slow)

### Step 3: Voice Compression

1. Insert a compressor on the vocal track.
2. Start with **2:1 to 4:1** ratio.
3. Lower threshold until you see **3–8 dB** of gain reduction on louder phrases (more if the performance is very dynamic).
4. Adjust attack/release to control consonants and sustain:
   - Too fast attack can dull clarity and make “T/K/P” less present.
   - Too slow attack can let peaks poke out and feel inconsistent.
5. Level-match output and A/B.

Goal: the vocal stays forward and intelligible without sounding squashed or obviously “grabby.”

### Step 4: Comparison and Analysis

1. Pick one source (kick, room mics, drum bus, or vocal).
2. Copy your starting settings idea (ratio/attack/release targets) and repeat the process using a **different** compressor plugin.
3. Level-match and A/B:
   - Which one changes the tone more?
   - Which one feels smoother vs. punchier?
   - Which one makes you fight the mix less?

Write down what you preferred and *why* (one or two sentences per source is enough).
