+++
title = "Compression"
outputs = ["Reveal"]
[reveal_hugo]
custom_theme = "reveal-hugo/themes/sunblind.css"
margin = 0.2
+++


## Introduction to Compression

- Definition: Compression as an automated fader
- Purpose: Reducing undesirable signal-level variations
- Example: Correcting vocal level inconsistencies
- Compressors' role in achieving a balanced mix

{{% note %}}

- **Role of Compression**: Helps achieve a balanced mix by managing dynamic range.  
- **Dynamics Control**: Reduces level differences, ensuring all elements are audible without excessive volume shifts.  
- **Stable Balance**: Addresses signal-level variations when a static fader position doesn’t work.  
- **Glueing Elements Together**: Mix bus compression enhances cohesion, making sounds interact dynamically.  
- **Individual Instrument Compression**:  
  - Evens out bass guitar notes.  
  - Ensures vocals remain consistently heard.  
  - Makes drum hits more uniform.  
- **Mix Buss Compression**: Helps unify the mix by creating subtle interactions between elements.  
- **Compression as an Indicator**: Bus compression acts as a "soft ceiling," highlighting arrangement clashes.  
- **Caution Against Over-Compression**: Can alter timbre, introduce noise, and make the mix sound lifeless. Use compression judiciously.

{{%/ note %}}

---

![](fig-9.1.png)

---

# Key Compression Controls 

- Threshold
- Makeup Gain
- Ratio
- Attack and Release

---

## Threshold and Makeup Gain 

- Threshold: sets the level where compression begins
- Peak Reduction vs. Input Gain
- Makeup Gain compensates for volume lost during compression
- Beginners: start with Threshold or Peak Reduction controls

{{% note %}}

## Threshold 

*   **Definition:** Threshold is a primary parameter that governs the activity of the side-chain in dynamics processing. It represents the **level at which a dynamics processor begins to adjust gain**. The threshold determines the point where the compressor starts turning the volume down.
*   **Function in Compressors:**
    *   The threshold setting determines the level at which the compressor will begin to proportionately reduce the incoming signal.
    *   Signals **below the threshold remain unaffected**, while those **above are attenuated**.
    *   Some compressors feature a **fixed threshold level**. In this case, the amount of compression is set by varying the input signal's level relative to that threshold. The more the signal exceeds the fixed threshold level, the more compression occurs.
    *   The threshold can be adjusted to control the level of compression. Turning the threshold knob down increases the amount of compression, while turning it up decreases the amount of compression.
*   **Function in Expanders:** For expanders, signals **below the threshold** have gain reduction applied to them.
*   **Knee:** Most quality compressors offer hard and soft knee threshold options. A soft knee widens the threshold range, making the onset of compression less noticeable, while a hard knee setting causes the effect to engage quickly above the threshold point.
*   **Dynamic EQ**: In Dynamic EQ, the threshold setting defines the relative threshold, or difference, between broadband and bandpass levels, which result in compression of sibilants.
*   **Gain control**: On some devices, varying the input gain will correspondingly control the threshold level.
*   **Threshold as a trigger**: Each of the threshold controls acts like a trigger or hinge point, activating gain reduction or expansion only when the input signal exceeds the set point value.


## Peak Reduction and Input Gain

*   **Peak Reduction**
    *   A control labeled "Peak Reduction" (or sometimes just "Compression") increases compression, resulting in more reduction of peak levels, as it is turned up.
*   **Input Gain**
    *   With an Input Gain control, the compressor has a **fixed threshold level**. The amount of compression is set by **varying the input signal’s level relative to that threshold**.
    *   Turning up the Input Gain control causes the signal to exceed the fixed threshold level, resulting in more compression. However, the **signal’s overall level also increases** as more compression is added.
*   **Key Differences**
    *   **Level Increase**: **Input Gain increases the overall signal level** as compression is added, whereas Peak Reduction typically makes the signal quieter when compression is applied.
    *   **Fixed Threshold:** Input Gain controls are used on compressors that have a fixed threshold.
    *   **Potential for Over-processing**: Input Gain can give a potentially misleading impression that processing is improving the sound due to the level hike, even if the amount of compression is excessive.
    *   **Versatility**: Becoming comfortable with both control types gives access to a wider choice of compressors at mixdown.

## Makeup Gain 

*   **Definition:** Make-up Gain is a control on a compressor that **boosts the output signal back up to its original level (or beyond)** after the compressor has reduced it. It controls the desired output level with compression active. It allows you to compensate for the loss in loudness caused by the compressor.
*   **Primary Function:** The most important thing when setting a compressor is using the Make-up Gain parameter.
*   **Maintaining Balance:** Make-up gain helps to **maintain the audible loudness and overall mix balance** when compression is applied. When the compressor is switched in and out of the signal path, the goal is to keep the sound in the same place in the mix.
*   **Avoiding Misleading Impressions**: It's important to adjust the compressor's Make-up Gain control to compensate for any loudness increase. This is done so that bypassing the compressor doesn't boost the subjective volume, which can mislead you into over-processing.
*   **Setting by Ear**: Because a compressor causes a loudness change that varies with time, it's best to set the make-up gain by gut feeling. If there are doubts about the amount of make-up gain, it’s better to use a bit less. This way, you're less likely to think the compressor has a positive effect, and it makes you work harder to really find the optimal setting.

## Practical Tips for Effective Use

- For beginners, it's recommended to start with Threshold or Peak Reduction controls to avoid misleading impressions of sound improvement due to volume increases associated with Input Gain control. Mastering these controls can greatly enhance mix balance without delving into complex technicalities.

{{%/ note %}}

---

## Identifying Tracks that Benefit from Compression

- Evaluating instability in track levels
- When fader adjustments are insufficient
- Instruments that commonly require compression
- Using automatic gain makeup: Pros and cons

{{% note %}}

- The decision to use compression should be based on whether it's impossible to achieve a stable mix balance with fader adjustments alone.
- A key indicator for needing compression is if you find yourself constantly adjusting a track's fader to maintain balance, such as with vocals where some phrases are too soft or too loud.
- While some instruments, like electric guitars, may not require compression due to their inherent characteristics, others, particularly vocals and bass, often benefit from it to maintain consistent levels throughout a performance.
- Compression is not always necessary, but in many modern music productions, it's essential for achieving the polished sound expected in commercial releases, addressing issues from uneven instrumental performances to the technical challenges posed by electronic and acoustic instruments.

## Automatic Gain Makeup: Pros and Cons

*   **Definition**: Automatic gain makeup is a feature in some compressors that automatically compensates for the level change that occurs when compression is applied.
*   **Pros**:
    *   It seems like a bright idea on the face of it, because it leaves one hand free.
*   **Cons**:
    *   Automatic gain makeup often encourages inexperienced users to overcook the processing.
    *   Automatic gain makeup designs almost always make compressed signals feel louder than uncompressed ones, which can mislead users into applying too much compression.
    *   The loudness hike probably helps manufacturers sell more plug-ins.
    *   The automatic option is not precise.

In summary, while automatic gain makeup may seem convenient, the sources suggest that it can lead to over-compression due to the perceived loudness increase. It may be preferable to manually adjust the gain to ensure more accurate control over the final sound. One should be super vigilant when matching the subjective loudness of the processed and unprocessed sounds for comparison purposes, because most loudness processors make it ridiculously easy to mug yourself in this way. It is essential to focus on the side effects, not the loudness hike. Therefore, manual adjustment is generally recommended for better control.


- From here, go to the mix and work on some of the tracks that you think might benefit from compression.

{{%/ note %}}

---

## Starting with Compression: Choosing the Right Compressor

- Model and price matter less than knowing how to use it
- Start with presets; aim for at least 6 dB gain reduction on peaks
- Goal: achieve a stable fader position in the mix
- If over-compressed, try a different compressor or preset

{{% note %}}

- Focus more on understanding how to use a compressor effectively than on the model or price. Both Tony Visconti and Bob Clearmountain emphasize that a compressor's function is largely uniform across different models.
- Start by inserting a compressor on the track in need, using presets as a starting point. Adjust the Threshold to achieve at least 6dB of gain reduction on peaks, and use Makeup Gain to compensate for level changes.
- The goal is to stabilize the track's level within the mix. If initial settings don't solve the balance issue, further adjust the Threshold, even exploring extreme settings, to find a stable fader position.
- Be cautious of over-compression, as it can detract from the mix's life and energy. If compression affects the track negatively, experiment with different compressors or presets to find the best fit. Remember, different compressors react differently to the same settings, providing a variety of tonal and dynamic outcomes.

{{%/ note %}}

---

## When to Look Beyond Compression

- Compression can't solve every balance problem
- Other processing techniques may be more appropriate
- Individual track compression offers more precise control than group compression
- Prioritize mix balance and musical quality above all

{{% note %}}

- Not all balance issues in a mix can be resolved with compression alone. If adjusting settings or switching compressors doesn't stabilize the fader, it might be a sign that compression isn't the right tool for the job.
- It's crucial to prioritize the mix's overall balance and sound quality over relying solely on compression to fix level inconsistencies. Other processing techniques may be more suitable for certain problems.
- When considering whether to compress individual tracks or a group channel, remember that compressing each track separately allows for more precise control over level imbalances. Group channel compression, while useful for glueing elements together, cannot correct individual tracks' standout issues.
- Ultimately, the decision on processing should be guided by the goal of achieving a well-balanced, musically pleasing mix, even if it means using a combination of techniques beyond compression.

{{%/ note %}}

---

## Refining Compression Settings: Ratio Control

- Ratio: how much compression is applied above the threshold
- Higher ratios reduce dynamic range more aggressively
- Example applications: slap bass, acoustic guitar
- Start moderate; adjust using the gain-reduction meter

{{% note %}}

## Definition 

*   **Definition**: Compression ratio is a control on a compressor/limiter that **determines how much compression or limiting will occur when the signal exceeds the threshold**. It sets how firmly the compressor reins in signals that overshoot the threshold level. It is expressed as a ratio of **input level to output level**.
*   **Function**:
    *   It effectively sets **how much the volume changes** once the signal exceeds the threshold setting.
    *   It determines the **slope of the input-to-output gain ratio**, which is the amount of input signal (in decibels) needed to cause a 1 dB increase at the compressor’s output.
*   **Ratio Explained**:
    *   A ratio of **1:1 results in no compression at all**. With a 1:1 ratio, the output tracks the input, meaning a 2 dB change at the input produces a 2 dB change at the output.
    *   A ratio of **4:1 means that for every 4dB that goes into the compressor, 1dB will come out**. For every 4 dB increase above the threshold point the output only increases 1 dB.
    *   A ratio of **10:1 or greater is considered limiting**. For a 10:1 ratio, a 10 dB blast at the input changes only 1 dB at the output.
    *   Some compressors offer **infinity:1**, meaning overshoots are effectively stopped in their tracks, unable to cross the threshold at all.
*   **Effect on Sound**:
    *   **Low ratios** (around 2:1) are suitable if you want the compression to sound smooth and controlled.
    *   **Higher ratios** (above 4:1) are appropriate if you want to hear the compressor work or if you want the sound to be punchier. The higher the compressor ratio control is set, the more likely you’ll hear the compressor or limiter work.
*   **Practical Considerations**:
    *   Different compressors can react quite differently for the same Ratio setting.
    *   It's more practical to use a compressor with a gain-reduction meter to see when and how much the compressor is working as you adjust the Threshold and Ratio controls.

In summary, **the compression ratio determines the degree to which the compressor reduces the dynamic range of a signal once it exceeds the threshold**. A higher ratio results in more aggressive compression, while a lower ratio provides more subtle dynamic control.

- For dynamic instruments like a slap bass, high ratio settings are necessary to firmly control sporadic peaks, ensuring they don't overpower the mix.
- Conversely, for instruments with a more consistent dynamic range, like an acoustic guitar, lower ratios provide gentle compression, maintaining musical dynamics while achieving a balanced level.
- The key to effective compression is finding the right ratio that addresses the balance issue without sacrificing the instrument's natural performance dynamics. This often involves starting with a moderate ratio and adjusting based on the effect observed through the gain-reduction meter, aiming for the least aggressive setting that achieves the desired balance.

{{%/ note %}}

---

## Understanding Attack and Release Times

- Attack and Release control how quickly the compressor responds
- Addressing transient vs. sustain level differences
- Too fast = over-compressed transients; too slow = missed peaks
- Adjust by ear; use the gain-reduction meter for visual feedback

{{% note %}}

- Attack and Release Time controls are essential for fine-tuning how a compressor responds to changes in the input signal, affecting the balance between transient and sustain elements of a sound.
- If a compressor reacts too quickly (short Attack and Release times), it may over-compress transient details, like the initial strum of a guitar, leading to a loss of natural impact and dynamics.
- Conversely, setting these times too slowly may fail to catch and properly reduce unwanted level spikes, making it challenging to achieve a balanced mix.
- The key to effective use of Attack and Release settings is to adjust them by ear, aiming for the best mix balance while minimizing adverse effects on the music's natural phrasing and dynamics. Visual feedback from a compressor's gain-reduction meter can aid in finding the right settings by showing the compressor's response to signal changes.

{{%/ note %}}

---

## Tailoring Drum Compression: Attack and Release Settings

- Small timing changes yield very different drum sounds
- Three configurations for snare drum compression
- Automatic vs. Manual Attack and Release Times
- Manual settings give more predictable, targeted results

{{% note %}}

- Adjusting Attack and Release times on a compressor allows for nuanced control over drum dynamics, offering different outcomes based on the settings chosen.
  - **Fast Attack, Fast Release:** This setting quickly reduces the gain of the initial drum transient but resets quickly, reducing the transient's impact while preserving the tail of the drum sound.
  - **Fast Attack, Slow Release:** A rapid onset of compression with a slow release maintains the balance between the drum's transient and sustain, enhancing overall hit consistency without altering the drum's natural dynamics significantly.
  - **Slow Attack, Slow Release:** Allowing the initial transient to pass before compression kicks in accentuates the transient while compressing the sustain, potentially increasing the dynamic range between the hit's peak and body.
- Automatic Attack and Release settings, while beneficial for managing complex sounds transparently, may not provide the precise control needed for specific sound shaping tasks, such as enhancing or reducing a drum's transient or sustain. Manual adjustments offer more predictable results, especially when targeting specific drum characteristics for a mix.

{{%/ note %}}

---

## Compressing Lead Vocals: A Step-by-Step Guide

- Vocals need a staged approach due to their wide dynamic range
- Stage 1: Split the track by dynamic range; use clip gain to pre-balance
- Stage 2: Soft-knee compression at 2:1–3:1 for transparent leveling
- Stage 3: Second compressor or limiter to catch remaining peaks
- Manual fader automation is still needed for final vocal presence

{{% note %}}

- Lead vocals often require a more nuanced approach to compression due to their wide dynamic range and the challenge of avoiding unnatural sound processing effects.
  - **Stage 1:** Divide the vocal track based on different sound qualities or dynamic ranges, using clip gain adjustments for preliminary level balancing.
  - **Stage 2:** Apply a first layer of compression with soft-knee settings around 2:1 to 3:1 ratio and moderate attack and release times for a transparent effect, aiming to even out the overall vocal levels without coloring the sound too much.
  - **Stage 3:** If necessary, apply a second layer of compression with faster, higher-ratio settings or a limiter for controlling remaining peaks, carefully adjusting attack and release times to avoid artifacts on consonant sounds.
- Despite the extensive use of compression, achieving the level of consistency expected in commercial releases often requires manual fader automation to fine-tune vocal presence and clarity, emphasizing consonants and phrases as needed.
- The goal is to balance effective dynamic control with maintaining the natural quality of the vocal performance, avoiding overprocessing by reserving detailed automation for later stages in the mixing process.

{{%/ note %}}

---

## Parallel Compression: Enhancing Dynamics

- Parallel compression blends processed and unprocessed signals
- Retains original track dynamics while controlling peaks
- Common in drums, piano, and acoustic guitar processing
- Avoids loudness bias by careful balance control

{{% note %}}

- Parallel compression, also known as "New York" compression, mixes compressed ("wet") and uncompressed ("dry") versions of a sound, preserving natural dynamics and transients while achieving desired loudness and tone.
- Especially beneficial for transient-rich instruments, this technique allows for aggressive compression without sacrificing the clarity of the original performance, keeping the music's dynamics lively.
- It's a favored technique among professionals for its ability to maintain the essence of the original sound while still benefiting from the sustain and body added by compression.
- To counteract loudness bias and ensure a balanced mix, it's recommended to group both signals and adjust their overall level together, preventing the common pitfall of overemphasizing the processed signal.
- In Reaper, we can do this using an FX container running in parallel with the original track, then controlling the wet/dry mix of the container.

{{%/ note %}}


