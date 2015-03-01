# Week4

## Dynamic Effect
Dynamic in general musical control of volume (like crescendo in the score).  
Musical dynamic is not only volume, it changes more.  

About Dynamic range

* top: celling -> cause distortion
* bottom: noise floor

Amplitude or loudness is represented by dBSPL. 0dBSPL is quietest audible sound.  
Human senses to hear the sound depends on environment. So it is important to measure the sound by digital devices (for accuracy).	

## Noise

* Acoustic noise: noise from floor
 * Listen carefully to the silence or room tone
 * move away from noisy sources like fans and windows
 * create an isolated space for recording
 * turn off noisy sources like A/C. TV
* Electrical noise: noise from gear(ex. microphone's self noise)
 * use fewer pieces of gear
 * use shorter cables
 * use balanced cables
 * turn off appliances and dimmers
 * use high quality gear

Avoid unnecessary gain to avoid the noise.

* boost level electrically as little as possible
* try to move the microphone close to the sound source, instead of increasing the gain
* choose a directional microphone

It's better to decrease the noise when recording phase than decrease it in mixing phase.  
Because noise is sometimes useful to fill the spectrum. If you use filter, the effect of noise also disappear.

## Distortion
When the loudness over the limit, the gears will start to cause the distortion.

* Distortion turns the volume variations into timbre variations
* Distortion makes a signal brighter (changes the wave shape)

Drive is gain control before a distortion stage (drive is just like volume control but it is going purposefully into this distortion threshold)

To avoid the distortion,

* Place your microphone carefully (if too close to the vocal, it'll cause the distortion)
* Use pop filter
* Be careful to the red lights at the top of the channel level

## Dynamic Range Manipulation

Dynamic range manipulation is control of loudness, it already exists in original sound (natural dynamic range).  
In the post production phase, we change it to emphasize/de-emphasize the sound.  
ex. to show the vocal in front of the guitar

The way to manipulate the dynamic range,

* macro scale: change the fader by automation
* micro scale: use program, algorithm  
it is used to deal with the transient (transient is the peak of sound (like drum kick or clap)). because the transient is too fast to manipulate by hand.


## Dynamic Processors Overview

* Compression: quiet to loud / loud to quiet
 * reduce dynamic range
* Expansion: loud is more loud/ quiet is more quite
 * emphasize dynamic range 

If you want to arrange the level of two vocals, you can use the pencil tool to raise up bottom of the vocal.  
Another way to do it is to use the rule (program).  
Dynamic processors are rule-based gain controls. The major parameters are the same, but the rules are different.

## Dynamic Processor Parameters

![dynamic processors parameters](./week4/dynamic_processors_parameters.PNG)

* analyze: take some sample (envelope) and calculate RMS.
* respond: control volume fader

* threshold: the level at which the processor starts to function (rate of input : output).  
it have to be set based on the input signal. Because quiet play never hit the threshold and the loud play is always compressed, it is not good.  

* ratio: how match functions is given once it crosses the threshold.
* attack: how fast the fader moves or the volume changes at the beginning of the sound when sound crosses the threshold. 
* release: how fast the fader moves or the volume changes when the signal crosses back through the threshold.

![ratio](./week4/ratio.PNG)

* neef: to give the function gradually
* look ahead: delay imposed on the signal

## Gate
It is noise gate. It will cut the sound below the threshold.

If attack is set too high on a gate, the transients will be softened as the volume swells in.  
Usually a gate attack/release is set low (because want to cut noise fast), but related to the sound itself.  

The attack and release is largely based on the sound itself. 
if swells in/out the high attack/release is appropriate, but the short and punchy like clap, quick (lower) attack and release is best.

## Downward Compressor
It is used to lower the sound.

If increasing the attack, the beginning of the notes are pronounced. and low attack make the sound more flat.

## Limiter
It is extreme downward compressor (the ratio set very high, above 10:1 and low attack time).
The role of limiter is stop peaks. It is the protective effector (for the audience).

But sometimes the limiter cause the distortion. To avoid it, we have to increase the attack/release. It is trade-off.

* For the limiter, low attack/release time is good, but it may cause distortion
* Increase the attack time, we can't limit the initial of sound.

Limiter function control the threshold associated with the gain control (lower threshold, bring up output).

## References

* [Processors](http://www.astralsound.com/processors.htm)
