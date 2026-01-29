---
title: "Drum Editing"
---

## Step-by-Step Guide for Drum Editing

### Using Stretch Markers

We're going to use the snare and kick drum as guides to add stretch markers to our project. We'll then use these stretch markers to quantize the drums to the grid.

#### Preparing the Project

- **Commit Tempo Map Changes**: If you're satisfied with your tempo map from the previous lesson, glue all media items to commit the stretch markers. This is necessary before adding new stretch markers for drum editing. Select all items and use the glue action (**Mac**: ⌘ + Shift + G, **Windows**: Ctrl + Shift + G).
- **Hide Non-Drum Tracks**: Open the Track Manager and hide all non-drum tracks from the Track Control Panel. This simplifies your workspace and makes it easier to focus on drum editing.
- **Arrange Drum Tracks**: If you haven't already, rearrange your drum tracks in a logical order from top to bottom: Kick, Snare, Hi-Hat, Toms, Overheads, Room. This organization makes editing more intuitive and efficient.
- **Zoom Tip**: Use marquee zoom to quickly zoom into specific sections for detailed editing. Hold **Mac**: Option + ⌘ + Right Click Drag, **Windows**: Ctrl + Alt + Right Click Drag to draw a selection box around the area you want to zoom into.
- **Configure Grouping Settings**: Set up your grouping preferences to enable simultaneous editing of all drum tracks. Configure these settings:
  - ✓ **Enable item grouping and track media/razor edit grouping**
  - **Uncheck** "Selecting one item selects group"
  - ✓ **Track media/razor edit grouping affects only items that start and end at the same time**
  - ![](select-one-item.png)
- **Group Items**: Select all drum tracks and group them together (right-click → Group). This allows you to edit one track and simultaneously apply changes to all grouped tracks.

#### Creating Project Versions for Comparison
- **Save Project As**: Use "Save Project As" to save the prepared project as "ProjectName_Slicing" (or "ProjectName_NoStretchMarkers"). This will be your baseline for the slicing method.
- **Save Again**: Immediately use "Save Project As" again to create "ProjectName_StretchMarkers". You'll work on this version first, then return to the slicing version later to compare both techniques.

####  Adding Stretch Markers to Snare Track
- **Select Snare Track**: Focus on either the snare top or snare bottom track within your project.
- Open the dynamic split dialogue **(shortcut: D)** and use the following settings:
  - ![](adding-stretch.png)
- **Add Stretch Markers**: Use the action "Add stretch markers to selected items and grouped items" to add stretch markers to the transients on the snare track.
- **Duplicate Kick Track**: Before adding kick stretch markers, duplicate one of your kick tracks and rename it something like "Kick Dupe". Consider coloring it differently (right-click track → Track Color) so you don't accidentally delete the wrong track. This is essential because the stretch marker process will remove the snare stretch markers you just added.
- **Add Kick Stretch Markers**: Select the duplicated kick track and repeat the dynamic split process to add stretch markers to the kick transients.
- **Delete Duplicate**: After the stretch markers are added, delete the duplicated kick track. Your original kick track will now have both snare and kick stretch markers. 

####  Ensuring All Hits Have Stretch Markers
- **Inspect the Song**: Go through the entire song and check for any kick or snare hits that are missing stretch markers.
- **Manual Addition**: If any hits are missing markers, add them manually in Reaper using "shift + w".

#### Adjusting Drum Hits
- **Enable Snapping**: Turn on the snapping feature and set the grid snap spacing as needed.
- **Manual Adjustment**: Manually adjust drum hits to align with the grid. This is useful for changing a few drum hits.

#### Quantizing Using Stretch Markers
- **Set Grid Spacing**: Before quantizing, ensure your grid is set to at least 8th notes. Adjust this in the Snap/Grid Settings to match your song's rhythmic content.
- **Handle Drum Fills**: If your song has sections with drum fills that are faster than 8th notes, avoid quantizing those sections. Make a time selection around the sections you want to quantize (excluding fills), then use "stretch markers in selected items within time selection" → snap to grid. This allows selective quantization while preserving the natural feel of fills.
- **Apply Quantization**: Right-click on a kick track and navigate to stretch markers -> stretch markers in selected items -> snap to grid (or use the time selection method above for selective quantization).
- **Check for Glitches**: Listen to the track for any glitches introduced by this process.
- **Remove Problematic Stretch Markers**: Use "option + click" to delete stretch markers causing glitches. Repeat until all glitches are removed. This part is really important to ensure that the song doesn't sound too robotic.


### Without Using Stretch Markers

####  Initial Preparation
- **Group Drums**: Ensure your drums are grouped for simultaneous editing.
- **Enable Necessary Options**: In the options menu, select:
  - Auto-crossfade media items when editing
  - Trim content behind media items when editing

#### Splitting Drum Tracks
- **Split Snare Track**: Use "Dynamic split items" on the snare track. Ensure you choose "split selected and grouped items" to apply the split to all drum tracks based on the snare. Set the leading and trailing pads to 3ms and deselect "fade pad".
- **Repeat for Kick Track**: Follow the same process for the kick track.
- **Select All Splits**: After working on the kick, if you need to work on the snare splits, double-click the snare track to select all of the snare splits.
- **Verify Split Positions**: Before quantizing (next step), ensure all splits align with actual transients. Misaligned splits will cause incorrect quantization.
- **Tip**: Temporarily disable snapping by holding the **Shift key** while moving splits.

####  Quantizing Drum Group
- **Select All Splits**: Before quantizing, select all of the split media items you want to quantize. The easiest way to select multiple items is to **right-click and drag** across the items you want to select.
- **Quantize to Grid**: Go to item → item processing → quantize item positions to the grid. Configure the following settings:
  - Quantize to: **1/8 notes**
  - ✓ **Move grouped items with selected items**
  - ✓ **Extend starts of items to overlap with earlier items by: 30 ms**
  - ✓ **Shorten earlier items if quantized items overlap by more than: 30 ms**
  - Leave "Quantize item ends and stretch item to fit" unchecked
- Click **Process** to apply the quantization.

####  Managing Crossfades
- **Inspect Crossfades**: Check that crossfades are not obscuring the transients of your snare or kick. Navigate between crossfades (**Mac**: ⌘ + ], **Windows**: Ctrl + ]).
- **Adjust Crossfades**: If a crossfade is out of place, move it by holding the **Shift key**.

####  Comparing Techniques
- After correcting glitches, compare the results from the stretch marker method and the non-stretch marker method. Determine which technique provides better results for these drums.

## Final Note: Gluing Your Edits

**For this assignment**, leave the stretch markers, splits, and crossfades in your project as-is. This allows for flexibility if you need to make adjustments.

**For professional projects**, once you're satisfied with your drum edits, you should glue all of your edited items together (**Mac**: ⌘ + Shift + G, **Windows**: Ctrl + Shift + G). This commits your edits and:
- Prevents accidentally moving or changing individual splits later
- Simplifies further editing and processing
- Creates cleaner, more manageable project files

Always make sure you're completely happy with your edits before gluing, as this process is difficult to undo.

