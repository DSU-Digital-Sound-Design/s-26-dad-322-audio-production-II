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
- **Use the Track Manager**: For projects with many tracks, use the Track Manager to efficiently organize and manage your folders.
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

#### Manual Correction

- **Access Manual Mode**: Click the **Manual tab** (third tab at the top of ReaTune's interface).
- **Track Pitch**: Click the **"Track Pitch" button** in the manual correction tab.
- **Capture the Phrase**: Play through the section you want to correct. Aim to capture a complete melodic phrase - typically 4-8 bars works well. ReaTune will record and display the pitch as a graph.
- **Zoom In**: Use your mouse wheel and cmd + mouse wheel to zoom into the captured vocals for precise editing.
- **Draw Corrections**:
   - It's beneficial to have a keyboard nearby to check the intended notes of the melody.
   - **Click and drag horizontally** to create correction bars across the notes you want to fix.
   - **Click and drag vertically** to move the bars up or down to the correct pitch. The bars should snap to the nearest note in your selected key.
   - Correct the pitch manually, ensuring you don't over-tune and lose the natural quality of the vocals. Some pitch variation is natural and desirable.

### Vocal Alignment

- **Understand the Recording**: This track includes multiple vocal tracks:
   - Lead vocal (already tuned)
   - Double-tracked vocal (slightly out of time with the lead)
   - Additional backing vocals (if present)
- **Marking the Words**:
   - If you're not familiar with the song, it can be helpful to manually add markers (for your reference only) at the start of every word. Write down the lyrics to help you identify new words in the waveform.
   - To better see the phrases, increase the peak size by pressing _shift + up_. This won't alter the volume of the track.

#### Using Dynamic Split

- **Prepare for Splitting**:
   - Select all vocal tracks except the lead vocal.
   - Bring up "Dynamic Split" (shortcut: D).
- **Configure Settings**:
   - Under **"Action To Perform"**, select **"Write stretch markers to selected items"** from the dropdown menu.
   - Set the **threshold** to control sensitivity - start with **-20 to -30 dB** for vocals. Lower values will detect quieter sounds.
   - The transient detection may not work perfectly due to the minimal level difference between the transient and silence.
   - Use _when gate opens_ and _when gate closes_ options to place markers at the start and end of the words.
   - It's better to create more markers than needed - you can easily delete extras during the alignment process.
   - Click OK to add stretch markers to selected items and review your tracks.

![](align-settings.png)

### Editing Stretch Markers

- **Moving Markers**:
   - Configure your mouse modifier preferences for moving stretch markers as shown in the image below.
   - To move one track's marker independently when tracks are grouped, hold **Cmd** while clicking and dragging.
    ![](move-markers.png)
- **Deleting Markers**:
   - To delete a stretch marker, use _Alt + click_ (not Option).
   <!-- - ![](remove-markers.png) -->
- **Adding Markers**:
   - There is no default shortcut for adding stretch markers. You'll need to either:
     - Set up a custom mouse modifier in Preferences (Actions > Show action list > search for "Item: Add stretch marker at mouse position")
     - OR place your playhead where you want the marker and use the action manually
- **Bulk Marker Removal**:
   - To remove multiple markers, select the item, make a time selection over the markers, and then use the action **"Item: Remove all stretch markers in time selection"**. Consider assigning this a shortcut like Ctrl+Option+Backspace.

### Backing Vocals

- Now align the backing vocals with the lead vocal. Add stretch markers to the beginning and end of each word.
- **Work on each track separately first**: Add stretch markers to each backing vocal track individually to ensure each word has the correct stretch marker placement. This gives you precise control over each track.
- **Then group and align**: Once all backing vocals have their markers, group them together and move the stretch markers to align all the backing vocal words with each other and with the lead vocal. 

#### Finalizing Alignment

- **Group Your Vocals**: After editing, group your vocals together.
- **Aligning**: Move the stretch markers of one vocal track, and the corresponding markers in the grouped tracks will align automatically.
- **Attention to Detail**: Remember, aligning vocals is not automatic. It requires patience, time, and a keen ear to detail.

#### Checking Your Work

- **Target Timing**: Backing vocals should start words within **10-20ms** of the lead vocal for tight alignment.
- **Use Loop Playback**: Set up a loop around a phrase and listen repeatedly to check the alignment by ear.
- **Avoid Over-Alignment**: Overly tight alignment (less than 5ms) can sound unnatural and robotic. Some natural variation is desirable and adds character to the performance.
- **Listen in Context**: Check your alignment both soloed and in the full mix to ensure it sounds natural.



