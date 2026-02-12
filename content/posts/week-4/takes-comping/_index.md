---
title: "Takes and Comping"
---

> Adapted from [#shorts - REAPER 7 - Convert Take Lanes to Fixed Item Lanes - YouTube](https://www.youtube.com/watch?v=Cs70Wle-BPM) and [Track Lanes & Comping in REAPER 7 - YouTube](https://www.youtube.com/watch?v=QKql5MD-dCA)

### Converting Takes to Fixed Item Lanes

By default, recording over a media item in Reaper creates takes. To use the track lanes and comping features in Reaper 7, you'll need to convert existing takes to fixed item lanes.

#### Step 1: Access the Action List

1. **Go to Actions** > **Action List**.

#### Step 2: Find and Execute the Conversion Action

1. **Search for 'Take Explode'** in the Action List search bar.
2. **Select all tracks** you want to convert, then run `Take: explode takes on selected tracks to fixed lanes.`

### Introducing Track Lanes

Track lanes are a Reaper 7 alternative to the traditional stacking of takes. To start recording with track lanes:

1. **Accessing Track Lanes**: Navigate to the options menu and find the 'Overlapping recording behavior' section.
2. **Enable Track Lanes**: Choose the 'Add Lanes (new lanes play exclusively)' option. New takes will now create separate lanes instead of stacking.
3. **Recording with Track Lanes**: Record additional takes — each new take creates a new lane.

### Basics of Comping

Comping lets you compile the best parts of different takes into a single track.

1. **Enable Comping**: Right-click on one of the yellow item lanes buttons and choose 'Comping' > 'Comp into new empty lane'.
2. **Create a Comp Lane**: Reaper adds a new lane for your compiled track.
3. **Select the Best Parts**: Play through your takes and drag to select the best parts from each lane.
4. **Refine Your Comp**: Listen to the comp track in real-time to check transitions between selections.
5. **Finalize Your Comp**: Right click and select 'Show/play only lane' to compress the takes into one item.

### Advanced Comping Techniques

1. **Switching Between Takes**: Click on a take to select it for playback, or use `T` for next take and `Shift + T` for previous take.
2. **Cropping to Active Take**: Once you've chosen the best parts, right-click > Take > Crop to Active Take (or `Shift + Cmd + T`).
3. **Saving and Comparing Comps**: Instead of cropping, you can save comps for comparison: right-click > Comp > Save as New Comp. Switch between saved comps using the `Comp takes: Activate next comp` action.
4. **Collapsing Lanes**: Toggle **Options > Show all takes in lanes (when room)** to collapse or expand lanes when you're done comping.
