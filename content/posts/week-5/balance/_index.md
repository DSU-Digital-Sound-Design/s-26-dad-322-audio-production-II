---
title: "Building the Raw Balance"
---

> See [Chapter 8: Balance](https://cambridge-mt.com/ms/ch8/) for Mike Senior's demo on creating balance.

# Balance 

- Mixing demands a clear, overarching game plan to make confident decisions.
- Learning to mix is a step-by-step process, analogous to learning to drive, starting with basic techniques before progressing to more complex, nuanced skills.
- The most important aspect of mixing is achieving balance, ensuring every important sound is clear and appropriately leveled throughout the mix.

# What order do you start mixing in?

- The sequence of mixing different instruments and sections in a production is crucial, significantly influencing the final sound quality.
- Establishing a logical starting point in the mixing process is vital for making sense of and effectively managing the mixing workflow.

## Start with the most important section

Before mixing the most important section, we should add markers or regions around each section so we can easily see where they start and end.

What is the most important section of this song?

> “I’ll start with the louder or bigger section [with] the most instruments . . . the chorus typically, or maybe the bridge” says Neal Avron, for instance. “And then the rest of it is kind of ‘unbuilding’ for the verses and the intros.”

After we pick the most important section we'll start the mix there. From that point we can mix the other sections related to that one, making sure to leave the most important section the loudest and most upfront.

We might design the dynamic structure of a mix like this:

![](dynamic-structure.png)

The choruses are the most important parts so we mix all of those first.

## Start with the Most Important Instrument

Now that we've chosen the structure our mix will take, we have to find the most important instrument. What is that for this song? We'll bring up this fader first, then decide what else is important and go in that order. If we go in the correct order, we can avoid over-processing when trying to fit instruments into the mix.

Let's each write down a list of what we think the most important instruments are, in order of priority. We'll discuss why and try to stick to our plan.

## A Basic three-step process for balancing

> - **Unwanted Low Frequencies:** Begin by removing any unnecessary low frequencies from each instrument's audio track. This step is crucial for maintaining clarity in the mix.
> - **Pan Control Adjustment:** Next, adjust the pan control to position the instrument appropriately within the stereo field. Proper panning contributes significantly to the perceived spaciousness and organization of the mix.
> - **Fader Level Setting:** Finally, set the fader level to achieve the desired prominence of the instrument in the mix. This step is about finding the right balance where the instrument sits well with others while contributing effectively to the overall mix.

### High-pass filtering

High-pass filtering is an essential process in mixing, primarily used for cleaning up the low end of the track by removing unnecessary low frequencies. Below is an overview of its importance, usage, and best practices in the context of mixing.

#### Function of High-Pass Filter:
- **Basic Operation:** A high-pass filter progressively attenuates frequencies below a user-defined cutoff frequency, effectively "cleaning" the low end of the track.
- **Slope Control:** The steepness of the attenuation is measured in decibels per octave (dB/octave). Common slopes are 6dB (1-pole), 12dB (2-pole), and 18dB (3-pole) per octave. More extreme slopes like 72dB/octave are available but can introduce audio artifacts.
- **Filter Designs:** Some filters offer a Resonance, Bandwidth, or Q control, providing a level boost at the cutoff frequency. However, for general mix cleanup, this feature is less relevant and should be set to minimum.

#### Practical Application in Mixing:
- **Choosing the Right Tool:** For mixing purposes, high-pass filters integrated into equalizer plugins are generally preferred for their transparency, as opposed to those with resonance controls more suited for sound-design tasks.
- **Setting the Cutoff Frequency:**
  - A practical method is to increase the cutoff frequency until a change in the sound's low end is noticeable, then slightly reduce it.
  - This approach ensures that unnecessary low frequencies are removed without compromising the instrument's essential character.
  - For home studios, using a spectrum analyzer can offer additional insight, especially when monitoring conditions are not ideal.
  
#### Specific Considerations:
- **Instrument-Specific Filtering:** While the technique is broadly applicable, take extra care with instruments that have significant low-frequency content, like kick drums, snares, and bass.
  - For these instruments, high-pass filtering can sometimes affect the attack or punch of the sound. Therefore, set the cutoff frequency lower than usual and listen carefully for any negative impact on the instrument's attack.

### Pan control adjustment

- **Subjective Nature:** Panning decisions in mixing often boil down to the mix engineer's personal taste, rather than adherence to a strict notion of stereo realism. While some engineers aim for a natural stereo panorama, mainstream record production frequently involves panning for technical reasons or based on the engineer's preference.
- **LCR (Left-Center-Right) Panning:** Some engineers advocate for LCR panning, positioning elements strictly at left, center, or right. This approach simplifies the stereo field but may not always provide the desired spatial depth or realism in the mix.

#### Technical Considerations and Strategies:
- **Central Positioning for Key Elements:** Vital musical elements like kick, snare, bass, and lead vocals are typically placed in the center. This ensures they are prominent in mono playback and benefit from the combined low-frequency response of stereo speakers.  
- **Mono Compatibility:** When panning, consider how the balance will change in mono or single-sided stereo. Panning towards the extremes can cause a 3dB level drop in mono, potentially making an instrument less audible or even inaudible in one earbud.
- **Opposition Panning:** Balance the stereo field by panning similar or complementary instruments to opposite sides. This technique, known as opposition panning, helps to maintain a balanced stereo image and ensures clarity and separation between similar instruments (e.g., hi-hat and shaker).
- **Call-and-Response Panning:** Push call-and-response elements to opposite sides to enhance interaction and contrast within the mix. This technique can be particularly effective with guitar riffs, sound effects, and backing vocals. 
- **Dynamic Panning:** Consider dynamic panning, where elements are positioned differently in various sections of the song (e.g., something panned left in the verse answered by something on the right in the chorus), as suggested by Bob Clearmountain. This approach adds variety and maintains interest throughout the track.

### Fader level setting

- **Foundational Step:** Setting levels is a fundamental step in mixing, crucial for preventing distortion and ensuring each track sits correctly in the overall mix.  
- **DAW Headroom and Noise Floor:** Modern DAWs use floating-point processing, which means individual channels won't hard-clip internally even if their meters go red. However, this doesn't mean you should ignore hot levels. Plugins (especially analog-modeled ones) can distort or behave unpredictably when hit too hard, and the master output will clip when converted for playback or export. Keep individual channels at healthy levels to maintain good gain staging throughout your signal chain.

#### Strategies for Level Setting:
- **Avoiding Overloading:** Despite the ample headroom, it's wise to avoid channel and bus overloads for practical reasons, like the ability to export unclipped mix stems.
- **Processor Level Impact:** The level at which signals hit mix processors (discussed later) can significantly affect the overall sonic character.

#### Importance of Diligent Level Balancing:
- **Time and Attention Requirement:** Balancing levels is a time-intensive task requiring close attention. It's essential not to rush this stage as it sets the foundation for the mix.
- **Monitoring and Reference Practices:** Employing good monitoring practices, using different listening setups, and occasionally referencing commercial tracks can provide a comprehensive perspective on the balance.
- **Balance and Trade-offs:** Achieving balance involves trade-offs between making each track audible and distinct without overshadowing others. Continuous assessment and adjustment are key to maintaining harmony among all mix elements.

#### Moving Forward with Level Setting:
- **Preliminary Decisions:** Make informed initial fader settings to minimize the need for extensive processing later. Stay attentive to the balance and be ready to employ plugins where necessary.
- **Ongoing Adjustment and Reference:** Understand that the initial balance is a starting point. The final, polished balance often requires ongoing adjustments, processing, and referencing against commercial productions for a well-rounded and competitive mix.

### Step-by-Step Mixing Process for a Rock/Pop Track

I'm going to demo this with a random track from [The 'Mixing Secrets' Free Multitrack Download Library
](https://cambridge-mt.com/ms3/mtk), but this process will work for other songs as well. 

#### Starting with Drums

Work through the drum kit from the most prominent elements to the supporting ones.

**Overhead and Room Mics:**
- **Initial Focus:** Start with the overhead tracks to establish the overall character and shape of the drum kit before dialing in individual drums.
- **Mono Compatibility Check:** Toggle mono on your master bus to listen for phase cancellation between the overheads and room mic, which are at different distances from the kit. If the sound thins out or loses punch in mono, try flipping the polarity on the room mic or time-aligning it to the overheads.
- **High-Pass Filtering:** Apply a high-pass filter and raise the cutoff until you hear the low end thin out, then back it off slightly. A starting point around 80-120 Hz is common for overheads.
- **Pan Adjustment:** Pan the left overhead left and the right overhead right to create a natural spread, typically around 70-80% each direction.
- **Level Setting:** Bring the overheads up until the drum kit has a sense of air and space without overwhelming the close mics you will add later.

**Snare:**
- **High-Pass Filtering:** Apply a high-pass filter conservatively. The snare has important low-mid body, so start the cutoff low (around 80 Hz) and listen carefully. Avoid cutting into the fundamental if it diminishes the snare's weight.
- **Pan Adjustment:** Place the snare at or near center. Slight offset (10-15%) toward the hi-hat side can feel more natural but is not required.
- **Level Setting:** Set the snare loud enough to cut through clearly. The snare is often the anchor of the groove, so treat its level as a key reference point for the rest of the drum mix.

**Kick Drum:**
- **High-Pass Filtering:** Apply a high-pass filter very carefully. The kick carries essential sub and low-mid energy. Start the cutoff below 40 Hz to remove only true subsonic rumble, then use a spectrum analyzer to confirm you are not removing audible punch.
- **Pan Adjustment:** Keep the kick centered.
- **Level Setting:** Balance the kick against the snare so neither dominates. They should feel like they share the same room. Check the relationship frequently by soloing both together.

**Hi-Hat and Cymbals (Close Mics, if present):**
- **High-Pass Filtering:** Hi-hats and cymbals have little useful low-frequency content. Set the high-pass filter cutoff to 300-400 Hz or higher to clean up bleed.
- **Pan Adjustment:** Pan the hi-hat to the side opposite the ride or floor tom to create a natural kit image. Use opposition panning to balance the stereo field.
- **Level Setting:** Bring these elements in to taste, supporting the groove without cluttering the high frequencies.

**Toms:**
- **High-Pass Filtering:** Apply a high-pass filter to each tom track, removing frequencies well below the tom's fundamental. Floor toms need a lower cutoff than rack toms.
- **Pan Adjustment:** Pan toms to reflect their physical position in the kit, moving from left (high tom) to right (floor tom) or vice versa depending on the kit orientation.
- **Level Setting:** Toms are typically lower in the mix except during fills. Set a level that lets them sit naturally when playing and cut through during fills.

#### Moving to Bass

- **High-Pass Filtering:** Apply a high-pass filter to remove any subsonic rumble or low-end noise. A cutoff around 30-40 Hz is typical. Use a spectrum analyzer to confirm you are only removing content below the instrument's fundamental range.
- **Pan Adjustment:** Keep the bass centered. A centered bass locks with the kick drum and ensures consistent energy in both mono and stereo playback.
- **Level Setting:** Bring the bass up until it supports and complements the kick drum. The two should feel like they occupy the same low-end space without fighting each other. Check the balance in mono to confirm the bass and kick remain distinct.

#### Mixing Guitars

**Rhythm Guitars:**
- **High-Pass Filtering:** Apply a high-pass filter aggressively on rhythm guitars. Guitar low-end often conflicts with the bass and kick. A cutoff around 80-120 Hz is a good starting point, though some engineers go higher.
- **Pan Adjustment:** If there are two rhythm guitar tracks (a common recording approach), pan them to opposite sides, for example 60-80% left and 60-80% right. This creates width and separation. If there is a single rhythm guitar, position it where it best balances the mix.
- **Level Setting:** Set rhythm guitars to support the groove and harmonic foundation without masking the bass or overloading the midrange. They should feel like part of the bed of the mix, not the lead element.

**Lead Guitar or Featured Guitar Parts:**
- **High-Pass Filtering:** Apply a high-pass filter similarly to rhythm guitars, adjusting the cutoff to preserve the body of the tone while removing low-end mud.
- **Pan Adjustment:** Position the lead guitar where it has space in the stereo field. Center works well if it is the primary melodic focus. An offset position can work if it is a secondary element responding to another instrument.
- **Level Setting:** The lead guitar should sit above the rhythm guitars and be clearly audible as the featured part. Use the vocals (when present) as a reference point so the lead guitar does not compete with them.

#### Finishing Up

- **Speaker Switching and Breaks:** Regularly switch between different listening setups (studio monitors, headphones, a small Bluetooth speaker) to check how the balance translates. Take short breaks to reset your ears. Return at a lower volume to confirm the balance still holds when you are not listening loud.
- **Final Level Check:** Before moving on, aim for a master track peak no higher than -6 dB. This leaves sufficient headroom for processing, bus compression, and mastering. If the master is peaking higher, bring all faders down together rather than adjusting individual tracks.
