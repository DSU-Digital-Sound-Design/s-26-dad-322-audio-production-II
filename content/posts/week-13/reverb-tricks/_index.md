---
title: "Other reverb tricks"
---

Here are some lesser known things you can do with reverb

## Gated reverb examples

This video goes into depth on how gated reverb was created and what songs use it.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Bxz6jShW-3E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

See [this playlist](https://open.spotify.com/playlist/5zh0IzdP530nxTKRmarv5q) of some famous uses of gated reverb. Some songs are from the original era and some are newer.

Here are some of my favorites:

<iframe width="560" height="315" src="https://www.youtube.com/embed/VerK4zwMRQw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/qALvRCFNNpo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/_mTRvJ9fugM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/QKYkZnxZ3ZA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/kKBCLHAq1do" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Gated Reverb in Reaper

We'll create our own drum pattern for this exercise. Download the starter project [here](https://dakotastateuniversity-my.sharepoint.com/:f:/g/personal/tate_carson_dsu_edu/Enr7MZracTtMlLZ8fTSGNY4BDfbOUMccFjfI1OLciLk85A?e=53hWc1). We have one track that routes its MIDI to three other tracks. We do this, so we can have more control over mixing each part of the drum machine. Create a gated reverb track and send the snare audio to it. Add a reverb to that track and adjust to your liking. Remember you can really overdo this because we're going to tame it with the gate later.

Add a ReaGate to the end of the FX chain on the reverb return. Adjust the threshold and release settings to taste. Try setting the release to 0 and adjusting the hold parameter for a more abrupt cutoff. Listen with the rest of the drums to get a reverb cutoff rhythm that sounds good.

Now do the same process for the other drum tracks. Create returns for each with their own reverb and gate settings. Feel free to use other reverb plugins.

## Dynamic reverb

We can control the reverb based on the audio its being applied to create dynamic reverb. In the same reverb project go to the folder called "Dynamic Reverb". The goal is to have the reverb louder when the singer isn't singing and bring it down when she is, creating a dynamic effect.

This is a reduced version of the [BraumXMedia song 'Koishii (feat. N.I.A.)'](https://cambridge-mt.com/ms/mtk/#BaumXmedia). Before adding the reverb do a rough mix so that the vocals stand out and the tracks are not clipping the master.

Add a "ReaVerbate" plugin directly onto the vocal track. Create a preset with a large room size and little dampening.

Pick a reverb wet value for the spaces. This should be too much for the vocals, but that's ok for now. Make sure the reverb wet parameter is "last touched". Open the parameter modulation window. Choose the sidechain option and select channels 1 and 2. Now set the baseline to the value you chose for your "reverb wet value for the spaces". Finally, change the direction to negative.

Bring down the "minimum volume" so that the green dot is averaging its position around the red dot. NOw adjust the strength parameter so that the reverb web value doesn't go all the way to -inf dB.

Don't forget to adjust the attack and release so that everything sounds good and rhythmic with the track.

## Reverse reverb

We'll now work with some tracks from Whitten And. Williams' [Lie to Me](https://cambridge-mt.com/ms/mtk/#WhittenAnd). We'll create a reverse reverb as an introduction to the song. First, duplicate the ukelele track. Next reverse the track by opening the item settings. Move the reversed track so that it ends right before the start of the other tracks. Delete everything but the end of the reversed track.

Add a large reverb to this track. Be sure to remove the dry signal from the reverb. Fade in the item to get a smooth reverb riser. Now right-click on the track and find "Render/freeze tracks". Choose to render the track to a stereo stem track. Now reverse this track again. Line up the loudest part of the reverb swell with the start of the track. Notice how the ukelele part repeats? Copy your reverb swell and add it to that part for extra interest.
