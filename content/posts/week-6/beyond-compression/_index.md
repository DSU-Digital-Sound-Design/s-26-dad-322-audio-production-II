+++
title = "Beyond Compression"
outputs = ["Reveal"]
[reveal_hugo]
custom_theme = "reveal-hugo/themes/sunblind.css"
margin = 0.2
+++

## Expansion and Gating 

- Expansion increases dynamic range by lowering quiet sounds
  - Downward expansion reduces background noise and spill
  - Upward expansion enhances transients and attack
- Common uses: Reducing background noise and spill in recordings
- An expander's interface includes Threshold and Ratio controls
- Use of expansion and gating for balance and signal quality

{{% note %}}

- Expansion is the opposite of compression, aimed at enhancing the dynamic range by reducing the volume of softer sounds, thereby making the mix clearer.
- Expanders are valuable for minimizing unwanted sounds such as background noise or instrument spill, improving the clarity and focus of the main audio elements.
- The controls on an expander are straightforward, with the Threshold determining what gets reduced and the Ratio controlling the intensity of the reduction. Ratios vary from subtle to extreme, where extreme settings effectively mute the signal, turning the expander into a gate.
- Successful use of expansion requires careful evaluation of its impact on the balance and quality of the audio. If the desired outcome isn't achieved with basic settings, experimenting with different expanders or presets may be necessary. The goal is to solve balance issues without compromising the naturalness of the sound.

{{%/ note %}}

---

![](gate.png)

---

## Managing Gate Chattering 

- High-ratio expanders or gates can cause rapid gain fluctuations
- Chattering: Unmusical distortion, similar to stuttering audio
- Solutions include adjusting ratio, attack/release times, or using Hold Time control
- Hysteresis: Separate thresholds for gain reduction and reset to prevent chattering

{{% note %}}

- Using high-ratio expanders or gates with fast settings can lead to "chattering," where audio rapidly fluctuates, resulting in distortion or an awkward stutter.
- To counteract chattering, the first step might be to moderate the ratio or the attack/release times. However, in cases where sharp cutoffs are needed (like abruptly ending a snare drum's tail), this approach might not suffice.
- Introducing a Hold Time control can provide a buffer after the gate opens before it closes again, smoothing out transitions and reducing chattering. Even a brief Hold Time can significantly mitigate this issue.
- Hysteresis offers an advanced solution by establishing separate thresholds for activating and deactivating gain reduction, preventing the gate from reacting too sensitively to signals near the threshold. Adjusting the Hysteresis control carefully can eliminate chattering without compromising the desired sound quality or effect.

{{%/ note %}}

---

## Parallel Processing and Range Control 

- Parallel processing extends expansion/gating capabilities
- Tackles issues like hi-hat spill in snare recordings
- Parallel setup allows control over spill without altering dynamic range
- Range control limits maximum gain reduction, offering flexibility

{{% note %}}

- Parallel processing, familiar from compression applications, is also effective for managing expansion and gating challenges, such as hi-hat spill in snare drum recordings. By applying expansion in parallel, you can reduce unwanted spill while maintaining important aspects of the sound.
- This technique involves processing a duplicate of the original signal with high-ratio expansion or gating to eliminate unwanted sounds (like hi-hat spill), and then blending this processed signal with the original. This way, the balance between the snare and hi-hat can be finely adjusted without affecting the hi-hat's natural dynamics.
- Parallel expansion is particularly useful for emphasizing drum transients. By isolating and enhancing the initial attack of drum hits, you can add punch to the drum mix, making the overall sound more dynamic and impactful.
- Some expanders and gates feature a Range control, which sets the limit for how much the signal can be reduced. This allows for precise control over the amount of spill or unwanted noise in the mix, providing a versatile tool for mixing engineers to achieve the perfect balance between cleanliness and naturalness in recordings.

{{%/ note %}}

---

## Reshaping Drum Envelopes with Gating

- Hold Time control offers extensive delay range for creative gating
- Technique enables dramatic remodeling of drum sound envelopes
- Settings adjustment: Attack, Hold, and Release Time for tailored sound profiles
- Application: Enhancing programmed drums' dynamics and realism

{{% note %}}

- The extended range of Hold Time settings on expanders and gates is not just for preventing chattering. It's a powerful tool for creatively reshaping the dynamic profile of drum sounds, particularly useful for programmed drum parts that lack natural variation.
- By setting a high threshold to ensure the gate reacts to each drum hit, you can manipulate the Attack, Hold, and Release Time controls to redefine the sound's envelope. This allows for precise sculpting of the drum sound, from eliminating the initial attack for a softer onset to shortening or lengthening the sustain and decay phases for stylistic effect.
- Adjusting the attack time can effectively soften the impact of each hit, creating a more blended or subdued drum sound. Modifying the hold time alters the sustain duration, offering the ability to craft tighter or more expansive drum sounds. The release time adjustment enables control over how quickly the sound fades, providing options for both abrupt and smooth decays.
- This gating technique is especially valuable for adding dynamic interest and a sense of realism to electronic or programmed drum tracks, where natural level variations are minimal. By carefully adjusting these parameters, producers can achieve a wide range of sonic characteristics, from vintage drum machine textures to more organic, live-sounding drums.

{{%/ note %}}

---

## Transient Enhancers 

- Various techniques exist for emphasizing drum attack transients
- Digital recording challenges: Maintaining smoothness in transients
- Transient enhancers offer specialized, threshold-dependent processing
- Applications include upward expansion and dynamic gain boosting

{{% note %}}

- The quest to emphasize the attack portion of drum sounds has led to the use of various techniques, including slow-attack, fast-release compression, and high-threshold expansion. However, the transition to digital recording introduced new challenges, as digital tends to preserve transients more sharply than analog, leading to a need for more nuanced transient management.
- Transient enhancers are specialized tools designed to modify the transient characteristics of sounds in a mix, addressing the "in-your-face" quality of digital recordings. These tools can smooth out or accentuate transients to fit the desired mix context.
- One type of transient enhancement involves upward expansion or decompression, which increases the dynamic range of signals above a set threshold, selectively boosting signal peaks for greater impact. However, this can highlight inconsistencies in peak levels, which might not always be desirable.
- Another approach uses transient detection to apply a momentary gain boost, enhancing the attack phase of the sound. Some plugins also offer a second "sustain" envelope, triggered when the signal falls below the threshold, allowing for dramatic increases in sustain for elements like drum hits or repetitive synth parts. This flexibility makes transient enhancers a valuable tool for achieving the perfect balance and impact of transients in a mix.

{{%/ note %}}

---

## Threshold-Independent Transient Enhancement

- Limitation of threshold-dependent enhancement on complex tracks
- Transient detection without a threshold for more reliable processing
- Applications include modifying attack and sustain of acoustic instruments
- Comparing transient processors to find the best fit for each mix

{{% note %}}

- Threshold-dependent transient enhancement works well for signals where transients stand out significantly in level compared to the rest of the track. However, this approach falls short with complex, transient-rich material like acoustic guitar or piano, where not all transients exceed the surrounding signal level.
- An alternative, threshold-independent method detects transients based on the rate of level change, regardless of their absolute level. This allows for more consistent and versatile transient shaping, enabling users to either boost or reduce the attack of sounds without relying on a fixed threshold level. The same principle applies to managing the sustain phase of sounds, providing a comprehensive tool for dynamic shaping.
- Professionals like Jason Goldstein and Jack Joseph Puig have leveraged this type of processing to achieve specific sonic characteristics, such as reducing the 'plucky' quality of rhythm acoustic guitars or enhancing the attack for a more engaging and vibrant mix. This approach can make instruments stand out in the mix without necessarily increasing their overall volume.
- While many DAWs may not include these sophisticated transient processors by default, a variety of third-party plugins are available that offer this capability. It's important to note that these processors can vary significantly in how they detect and enhance transients, so experimenting with different options on your system is crucial to find the most effective tool for each specific mixing task.

{{%/ note %}}

---

## Tempo-Driven Balancing 

- Utilizing gain changes in sync with song tempo
- Techniques for enhancing rhythm parts without affecting sustains
- Methods include multing, MIDI-driven dynamics plugins, and tempo-synchronized effects
- Importance of phase control for matching DAW grid timing

{{% note %}}

- Tempo-driven balancing is a sophisticated technique for dynamically adjusting the levels of specific elements in a mix, such as emphasizing off-beat guitar chords without altering their sustain characteristics. This method requires the music to be aligned with the DAW's metric grid for effective implementation.
- One approach to achieving tempo-driven dynamics is multing: splitting the audio part across multiple tracks to independently adjust the levels of different rhythmic elements. This technique can be refined by fading edits to ensure smooth transitions and can accommodate complex rhythmic patterns beyond standard time signatures.
- Another method involves using dynamics plugins that respond to MIDI input, allowing for precise control over gain changes according to a programmed MIDI pattern. This can be particularly useful for gating rhythm parts or applying dynamic effects that match the song's tempo.
- Dedicated tempo-synchronized effects, such as gating, chopping, or tremolo, offer another layer of control, enabling adjustments to the dynamics and transient shaping of instruments or samples. These effects often come with a variety of modulation waveforms and may include a phase control feature, allowing for finer alignment with the musical timing, especially for parts that might not strictly adhere to the grid.
- Additionally, lookahead features in some dynamics processors can preemptively adjust to incoming signals, ensuring that transients are fully captured and processed without delay. However, caution is advised as lookahead can sometimes interfere with a DAW's plugin delay compensation, potentially leading to phase issues in parallel processing scenarios.

{{%/ note %}}

---