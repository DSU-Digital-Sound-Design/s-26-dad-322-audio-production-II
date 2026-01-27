---
title: "Tempo mapping in Reaper"
---

Continue working with the `Living in the City` project from the previous session. Before mixing, we need to establish an accurate tempo map so that Reaper's grid aligns with the song's actual tempo.

## Why Tempo Mapping Matters

When a song wasn't recorded to a click track, Reaper's grid won't match the performance. Tempo mapping solves this by adjusting Reaper's tempo to follow the recording. Once complete, you can:
- Edit precisely on the beat
- Add virtual instruments that stay in sync
- Use time-based effects (delays, reverbs) that match the song's feel
- Play a metronome that follows the performance

## Setup

### 1. Check the Recording

First, determine whether the song was recorded to a click:
- **Recorded to a click:** The tempo is constant—simply set Reaper's tempo to match and verify alignment.
- **Not recorded to a click:** The tempo fluctuates naturally, requiring manual tempo mapping (covered below).

## Implementing Tempo Mapping

### 1. Prepare Your Environment

- **Install the SWS Extension**: Download and install the [SWS / S&M Extension](https://www.sws-extension.org/) package if you haven't already. This provides the tempo mapping tools we'll use.
- **Configure Timebases**: Set your project timebases to ensure items stay in place during tempo changes:

![Timebase Configuration](../timbe-base.png)

- **Set Grid to Quarter Notes**: In Reaper's _Snap/Grid_ settings, set divisions to 1/4 notes. This gives you clear visual reference points for each beat.
- **Estimate the Starting Tempo**: Set an approximate tempo so that the first downbeat of the song lands on measure 2 of the Reaper grid. This leaves measure 1 free for any count-in.

### 2. Clean Your Timeline

Remove any silence at the beginning of your timeline so that the audio starts precisely at measure 2. Select the empty region before your audio and use `Cmd + Shift + X` (or right-click > "Remove contents of time selection") to delete the empty space.

### 3. Choose a Reference Track

Solo an instrument that plays consistently throughout the song—the snare drum or hi-hat works well. This gives you a clear rhythmic reference to align your markers against.

### 4. Mark Each Downbeat

1. **Show the Tempo Envelope**: Go to View > Tempo Envelope to visualize tempo changes as you work.
2. **Add markers on each bar**: Play the track and press `M` at the downbeat of each measure. Don't worry about precision on the first pass—you can adjust marker positions afterward by dragging them.
3. **Convert markers to tempo**: Open the Actions menu (`?`) and search for "SWS: Convert project markers to tempo markers". Run this action to transform your markers into tempo changes.

> **Important**: Complete this step before adding any organizational markers (verse, chorus, etc.), since the conversion affects all markers.

### 5. Verify Your Tempo Map

Enable Reaper's metronome and play through the song. The click should now follow the performance. If sections drift out of sync:
- Delete the incorrect tempo markers
- Re-mark those sections more carefully
- Run the conversion action again

## Trimming Silence

Now that the grid aligns with the music, it's easier to select items and verify edits land on musically meaningful points. Trim silence from each track to clean up the session and reduce bleed from other instruments.

This process is called "strip silence" in other DAWs. In Reaper, use the **Dynamic Split** feature:

1. Enlarge the track vertically with `Shift + !`
2. Press `D` to open the Dynamic Split Items dialog
3. Configure the settings:
   - Enable "When gate opens" and "When gate closes"
   - Leave "At transients" disabled
   - Adjust the gate **Threshold** until desired material reliably opens the gate
   - Set **Minimum slice length** and **Minimum silence length** to prevent very short regions
   - Enable "Remove silent areas (requires splitting on gate close)"
   - Check "Fade pad" with **Leading pad** and **Trailing pad** at 20 ms

![Dynamic Split settings](../split-silence.png)

4. Preview the result, then click "Split" to apply

Finish by soloing each track and listening to ensure no intentional material was removed and that note onsets and decays sound natural.

## Label Song Sections

With tempo mapping and cleanup complete, add markers and regions to identify song sections (as introduced in the previous session):

1. **Add section markers**: Press `M` to insert a marker, then name it (Intro, Verse 1, Chorus, etc.)
2. **Create regions**: Make a time selection over a section and press `Shift + R` to create a region
3. **Manage markers/regions**: Open the _Region/Marker Manager_ (View > Region/Marker Manager) to rename, reorder, or delete items

These markers make navigation easier during mixing and help you quickly jump between sections using the marker shortcuts or the Region/Marker Manager.
