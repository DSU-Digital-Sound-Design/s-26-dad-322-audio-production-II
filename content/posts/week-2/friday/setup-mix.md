---
title: "Importing and Organizing Audio Projects in Reaper"
---

Download the [Living in the City](https://cambridge-mt.com/ms/mtk/#HurrayForTheRiffRaff) mix from Cambridge Multi-tracks. After downloading your project, create a new Reaper project. Configure your project settings to mirror the following:

![](../project-settings.png)

Begin by reviewing the notes accompanying the tracks to determine the correct BPM (Beats Per Minute). Next, import your tracks into the project, ensuring they are sequentially ordered and color-coded based on the type of track.

Group similar tracks into dedicated folders. For instance, consolidate all drum tracks into a 'Drums' folder, and all guitar tracks into a 'Guitars' folder, and so on. Employ the track manager for efficient organization of projects with an extensive number of tracks.


## Trimming Silence

The next phase involves refining each track by eliminating silences and reducing bleed from other instruments captured by the microphone. Trimming unnecessary audio cleans up the session and encourages closer, more critical listening to the material. Address any obvious recording issues at this stage before beginning the mix.

This process is often referred to as “strip silence” in other DAWs.

In REAPER, this is accomplished using the Dynamic Split feature. To begin, enlarge the track vertically using Shift + !, then press D to open the Dynamic Split Items dialog.

Configure the dialog as follows:

* Enable “When gate opens” and “When gate closes”
* Leave “At transients” disabled
* Adjust the gate Threshold until desired material reliably opens the gate
* Set Minimum slice length and Minimum silence length to prevent very short regions
* Enable “Remove silent areas (requires splitting on gate close)”
* Check “Fade pad” 
* Set Leading pad to 20 ms
* Set Trailing pad to 20 ms

Once the preview looks correct, click “Split” to apply the edits.

Use the settings shown below as a reference:

![](../split-silence.png)

Finish by soloing each track and listening carefully to ensure that no intentional material has been removed and that note onsets and decays remain natural.


## Color-Coding and Track Renaming

Color-coding and renaming tracks are essential for maintaining a clear overview of your project. This practice enhances your workflow and helps you quickly identify specific tracks. For instance, you might color-code all drum tracks in blue, guitar tracks in green, and vocal tracks in red. This visual organization simplifies the mixing process and streamlines your workflow. You can also rename tracks to reflect the instrument or part they represent, such as "Kick Drum" or "Lead Guitar." 

## Regions and Markers

> Note: We would usually do this now, but in the next section we'll be doing some tempo mapping that will change the project length, so we'll wait until after that to set up regions and markers. Right now, just familiarize yourself with how to create them.

Regions and markers are indispensable tools for navigating your project. Regions are used to define sections of your project, such as verses, choruses, and bridges. Markers, on the other hand, are used to highlight specific points in your project, such as key changes or significant events. By utilizing regions and markers effectively, you can easily navigate your project and make precise edits and adjustments.

Use the following shortcuts to create regions and markers:
- To create a region: make a time selection and type `shift + R`
- To create a marker: `m`

## Utilizing a Reference Mix

1. Create a folder containing all your project tracks.
2. Place your reference mix track outside this folder. Ensure that this track does not route through your master channel if you're using any master effects.
3. Calibrate the loudness of your reference mix using a LUFS Meter, balancing between the readings of the meter and your auditory judgment.
4. Facilitate comparison (A/B testing) between your mix and the reference mix. In Reaper, you can solo tracks exclusively using option + command.
5. Consider adding additional reference tracks as needed.