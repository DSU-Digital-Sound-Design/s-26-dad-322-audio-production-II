---
title: "Tuning and Aligning Vocals"
---

### Overview

This page focuses on two essential aspects of vocal production: tuning and aligning vocals. We'll be practicing these skills using Benjamin John's song "Better Way". First, we'll tune the vocals using the ReaTune plugin, ensuring they are in the correct key and pitch-perfect. Then, we'll align the background vocals with the lead vocal.

### Preparing the Track

**Download the Track**: Start by downloading the full multitrack of Benjamin John's [Better Way](https://cambridge-mt.com/ms/mtk-newbies/#BenjaminJohn) to use in your class.

### Organizing Tracks into Folders

Before we begin tuning and aligning, organize your tracks for a cleaner, more efficient workflow. Arrange tracks by importance, with the most critical elements of a pop song at the top:

> **Workspace Tip**: Keep the mixer closed while editing. Since we're focusing on editing rather than mixing, closing the mixer (View → Mixer, or shortcut: Cmd+M / Ctrl+M) saves valuable screen real estate and helps you focus on the waveforms and editing tools.

- **Group by Instrument Type**: Create folders for similar instruments, ordered by importance from top to bottom:
  1. Vocals (Lead vocal, backing vocals, doubles)
  2. Guitars
  3. Piano/Keys
  4. Drums
  5. Bass
  6. Other instruments (synths, strings, etc.)
  - **How to create a folder**: Select the tracks you want to group, then right-click on one of them and choose "Create folder containing selected tracks" (or shortcut: Shift+Cmd+G / Shift+Ctrl+G).
- **Use the Track Manager** (View → Track Manager): For projects with many tracks, use the Track Manager to efficiently organize and manage your folders. This gives you a bird's-eye view of all tracks and makes bulk operations easier.
- **Color-Code**: Consider color-coding each folder for quick visual identification (right-click folder → Track Color).
- **Rename Tracks**: Make sure each track is clearly labeled (e.g., "Lead Vocal", "BV1", "BV2" instead of generic names).

This organization prioritizes the most important elements of a pop song and makes it easier to focus on the vocal tracks we'll be working with while keeping the project tidy.

### Tuning Vocals with ReaTune

#### Setting Up ReaTune

- **Add ReaTune Plugin**: Add the ReaTune plugin to your lead vocal track.
- **Solo the Track**: Solo your lead vocal track (click the solo button on the track) to hear it clearly while pitch correcting. This helps you focus on the pitch without distraction from other instruments.
- **Determine the Song Key**:
   - Click the **Tuner tab** (first of three tabs at the top of ReaTune's interface)
   - Set **Window size to 200ms** and **Overlap to 8x** for stable, accurate readings
     - **Window size** defines how much audio ReaTune analyzes at once - larger values (like 200ms) provide steadier, more stable readings by averaging over more audio
     - **Overlap** determines how frequently the analysis updates - higher values (like 8x) give smoother, more responsive readings at the cost of more CPU usage
   - **Enable monitoring**: At the bottom left of ReaTune, you'll see a dropdown that says "off" - change it to **"auto"** or **"on"** so you can hear the audio being analyzed.
   - Play through the song - watch the display:
     - The **upper section** shows the note name being detected
     - The **lower section** shows pitch in Hz and cents
     - A **green indicator in the center** means the note is in tune (left = flat, right = sharp)
   - Identify the key by noting which notes appear most frequently and feel like "home"
   - Once you know the key, click the **Correction tab** (middle tab) and select the key and scale from the dropdown menus. This will help you identify out-of-tune notes.

#### Configuring ReaTune

- **Set Attack Time**: Adjust the attack time to at least 50 ms to avoid an overly auto-tuned sound.
- **Mono or Stereo**: If your vocal is mono, disable stereo correction.
- **Choose Algorithm**: Set the algorithm to _Élastique 3.3.3 Soloist_ for the best quality. The Soloist mode is specifically designed for monophonic sources like vocals.

#### Automatic Pitch Correction

Before diving into manual correction, try automatic pitch correction first to see if it gives you acceptable results:

- **Stay in the Correction Tab**: Use the key you determined in the previous step with the tuner.
- **Enable Correction**: In the Correction tab, look for the slider at the top labeled "Correction amount" - move it up from 0% to 100% to enable automatic pitch correction. You can also adjust this slider to control how aggressively ReaTune corrects the pitch (100% = full correction, lower values = more natural but less precise).
- **Play Through**: Listen to how the automatic correction sounds. Pay attention to:
  - Does it sound natural or overly processed?
  - Are all the pitch issues being caught?
  - Are any correct notes being incorrectly "fixed"?
- **Adjust Attack Time if Needed**: If it sounds too robotic, increase the attack time further (try 100-150ms).

If automatic correction works well for your vocal, you may not need manual correction. However, manual correction gives you more precise control over individual notes.

#### Manual Correction

- **Access Manual Mode**: Click the **Manual tab** (third tab at the top of ReaTune's interface).
- **Track Pitch**: Click the **"Track Pitch" button** in the manual correction tab.
- **Capture the Phrase**: Play through the section you want to correct. Aim to capture a complete melodic phrase - typically 4-8 bars works well. ReaTune will record and display the pitch as a graph.
- **Zoom In**: Use your mouse wheel to zoom horizontally, and use **Cmd + mouse wheel** (Mac) / **Ctrl + mouse wheel** (Windows) to zoom vertically into the captured vocals for precise editing.
- **Draw Corrections**:
   - It's beneficial to have a keyboard nearby to check the intended notes of the melody.
   - **Click and drag horizontally** to create correction bars across the notes you want to fix - the bar will appear as a horizontal line showing what pitch the note will be corrected to.
   - **Click and drag vertically** to move existing bars up or down to the correct pitch. The bars should snap to the nearest note in your selected key.
   - **Delete Corrections**: To remove a correction bar, click on it to select it (it will highlight), then press the **Delete** key on your keyboard.
   - Correct the pitch manually, ensuring you don't over-tune and lose the natural quality of the vocals. Some pitch variation is natural and desirable.

#### After Tuning

Once you're happy with the tuning:
- **Leave ReaTune on the track** - Keep it active and processing. The pitch correction is applied in real-time.
- **Unsolo the track** - Click the solo button again to unsolo the lead vocal so you can hear it with other instruments.
- You can close the ReaTune window, but the plugin stays active in the FX chain.

### Vocal Alignment

Now that the lead vocal is tuned, we'll align the backing vocals. **The lead vocal will serve as our timing reference and will NOT be edited.**

#### Understanding the Vocal Tracks

This track includes:
- **Lead vocal** (29_LeadVox - already tuned) - This is your reference. Do NOT add stretch markers or edit this track.
- **Double-tracked vocal** (30_LeadVoxDT) - This will be aligned tightly to the lead vocal (separate from backing vocals).
- **Backing vocals** (31-46_BackingVox01-16) - 16 harmony tracks that will be aligned to each other first, then to the lead vocal.

#### Preparing for Alignment

- **Marking the Words** (optional but helpful):
   - If you're not familiar with the song, it can be helpful to manually add markers (for your reference only) at the start of every word. Write down the lyrics to help you identify new words in the waveform.
   - To better see the phrases, increase the peak size by pressing _Shift + Up Arrow_. This won't alter the volume of the track.

#### Using Dynamic Split to Add Stretch Markers

We'll use Dynamic Split to automatically add stretch markers to both the double track and all backing vocals.

- **Prepare for Splitting**:
   - Select the **double-tracked vocal (30_LeadVoxDT)** AND **all backing vocal tracks (31-46_BackingVox01-16)**.
   - Do NOT select the lead vocal (29_LeadVox).
   - Bring up "Dynamic Split" (shortcut: D).
- **Configure Settings**:
   - Under **"Action To Perform"**, select **"Add stretch markers to selected items"** from the dropdown menu.
   - Set the **threshold** to control sensitivity - start with **-20 to -30 dB** for vocals. Lower values will detect quieter sounds.
   - **Adjust Hysteresis**: Set hysteresis to help stabilize marker detection. If you need more markers, increase hysteresis; if you have too many, decrease it.
     - **What is hysteresis?** It creates different threshold levels for when the gate opens vs. closes, preventing the gate from rapidly opening/closing (chattering) when audio hovers near the threshold.
     - More hysteresis usually means fewer accidental opens/closes (more stable marker placement).
   - The transient detection may not work perfectly due to the minimal level difference between the transient and silence.
   - Use _when gate opens_ and _when gate closes_ options to place markers at the start and end of the words.
   - It's better to create more markers than needed - you can easily delete extras during the alignment process.
   - Click OK to add stretch markers to selected items and review your tracks.

![](align-settings.png)

#### Reviewing Dynamic Split Results

After Dynamic Split adds markers:
- **Zoom in** to see the markers clearly
- **Check visually**: Markers should be at the start of each word (look for waveform transients)
- **What to look for**:
  - ✓ Good: One marker at the beginning of each word
  - ✗ Bad: Multiple markers in the middle of a word (delete extras)
  - ✗ Bad: Missing markers on some words (add manually)
- Dynamic Split usually gets 80-90% of markers right - you'll likely need to add a few missing ones and delete some extras
- Don't worry about being perfect at this stage - you'll fine-tune during alignment

### Editing Stretch Markers

#### How Stretch Markers Work

When you move a stretch marker, the audio between markers stretches or compresses to match the new timing. Think of it like pulling or pushing audio to align with the grid or other tracks.

#### Moving Markers

- **Set up mouse modifiers** (only need to do this once):
?  - Go to Preferences (**Cmd+,** on Mac / **Ctrl+,** on Windows) → Mouse Modifiers
  - Context: **Media item stretch marker**, then set **left drag** to **Move stretch marker**
  - Optional (recommended): set **Cmd** (Mac) / **Ctrl** (Windows) to a behavior that **ignores selection/grouping**, so you can nudge one track without moving the whole group
  - See the image below for reference:
    ![](move-markers.png)
- **To move a marker**: Click directly on the stretch marker (small vertical line on the item) and drag left or right.
- **What to listen for**: As you move markers, listen for the words to align. The audio will stretch slightly to match the new position.
- **Move grouped markers together**: When tracks are grouped, moving one marker moves all corresponding markers on grouped tracks.
- **Move independently when grouped**: Hold the modifier you set above (often **Cmd** on Mac / **Ctrl** on Windows) while dragging to move just one track's marker.
- **Deleting Markers**:
   - To delete a stretch marker, use **Option + click** (Mac) / **Alt + click** (Windows).
- **Adding Markers**:
   - There is no default shortcut for adding stretch markers. You'll need to either:
     - Set up a custom mouse modifier in Preferences (Actions > Show action list > search for "Item: Add stretch marker at mouse position")
     - OR place your playhead where you want the marker and use the action manually
- **Bulk Marker Removal**:
   - To remove multiple markers, select the item, make a time selection over the markers, and then use the action **"Item: Remove all stretch markers in time selection"**. Consider assigning this a shortcut (e.g., **Cmd + Option + Backspace** on Mac / **Ctrl + Alt + Backspace** on Windows).
   - Menu path reference:
     ![](remove-markers.png)

### Aligning the Double-Tracked Vocal

The double-tracked vocal should be tightly aligned to the lead vocal, since it's meant to sound like a single, thicker vocal.

1. **Select only the double-tracked vocal**: Make sure you've added stretch markers to this track using Dynamic Split.
2. **Solo lead + double**: Solo both the lead vocal and the double-tracked vocal so you can hear them together clearly.
3. **Align to the lead**: Move the stretch markers on the double-tracked vocal to match the lead vocal's timing exactly.
   - The double track should start words within **5-10ms** of the lead vocal for a tight, unified sound.
   - Listen carefully - if it's too tight (under 2-3ms), it might sound artificially doubled. A little natural variation (5-10ms) often sounds better.
4. **Check for phase issues**: If the double track sounds thin or hollow when combined with the lead, try slightly offsetting the timing.

### Aligning the Backing Vocals

Now that the double-tracked vocal is aligned to the lead, we'll align the backing vocals in two stages:

#### Stage 1: Align Backing Vocals to Each Other

**Goal**: Get all backing vocals tight with each other first, before worrying about the lead vocal.

1. **Choose a reference backing vocal**: Pick one backing vocal track as your reference (usually the clearest or best-performed one).
2. **Group the backing vocals**: Select all backing vocal tracks and group them (right-click → Group).
3. **Align to the reference**:
   - **How to know where markers should be**:
     - Use your EARS first - loop a phrase and listen for when words start
     - Look at the WAVEFORMS - align the visual peaks (transients) of consonants across tracks
     - The goal is to make all backing vocals say the same word at the same time
   - Move stretch markers on the reference track to align with the lead vocal timing
   - Because the tracks are grouped, all backing vocal stretch markers will move together
   - This ensures all backing vocals are perfectly aligned with each other
   - **Visual check**: When aligned, the waveform peaks (word starts) should line up vertically across all tracks

#### Stage 2: Align Backing Vocals to Lead Vocal

**Goal**: Now align the tight backing vocal group to match the lead vocal timing.

1. **Keep backing vocals grouped**: Don't ungroup them - you've already aligned them to each other.
2. **Listen to lead + backing together**: Play both the lead vocal and your backing vocal group.
3. **Adjust backing vocal timing**: Move the stretch markers on your backing vocals to match the lead vocal's timing.
   - The backing vocals should start words at approximately the same time as the lead (within 10-20ms)
   - All backing vocals will move together because they're grouped 


#### Checking Your Work

- **Target Timing**: Backing vocals should start words within **10-20ms** of the lead vocal for tight alignment.
- **Use Loop Playback**: Set up a loop around a phrase and listen repeatedly to check the alignment by ear.
- **Avoid Over-Alignment**: Overly tight alignment (less than 5ms) can sound unnatural and robotic. Some natural variation is desirable and adds character to the performance.
- **Listen in Context**: Check your alignment both soloed and in the full mix to ensure it sounds natural.

