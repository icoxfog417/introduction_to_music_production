# Week6

## Synthesizer

* Oscillator: Create the (bright) sound
* Filter: remove unwanted frequency
* Amplifier: control the volume of the sound.(Synthesizer amplifier is designed to move the volume over time)
* Direct Control: manipulate the sound overtime by algorythm)
* LFO: control the cyclic parameter
* Envelope: control the key press(attack, delay, sustain. release)

## Oscillator

Oscillator creates the sound. Usually the first is bright sound, after the creation, adjust it.  

* Sine: pure tone. single frequency.
* Saw: series of upper partials or upper harmonics.
* Squre: like saw wave, but only the odd harmonics (saw wave is all harmonics).
* Triangle: sounds like filtered square wave (only includes the odd harmonics but they fall off faster as you go up the frequency spectrum).
* Noise: white noise etc (white noise is energy across the frequency and it's even across the frequency spectrum). 

## Filter

Low pass filter is very common. Because oscillated sound is usually bright.  
The filter works like mouth for vocal.

The resonance is related to the delay feedback. When resonance is high, we can notice the individual peaks of the individual harmonics as we sweep the cutoff frequency. 

* Low pass filter
 * low passed sound gets closet to the sine wave.
* Resonance
 * we can get peak right at the cutoff frequency, and as you seep that it will emphasize those individual harmonics drastically.
 * if you want the filter to remove the some frequency sound, then you don't need to use resonance.

## Amplifiers

Amplifiers work over time, and controls the volume (voltage control amplifiers). And the envelope is the path of  control.
Below key words have another meaning from usually context.

* Attack Time: the time to get from zero to full value when press the key
* Decay Time: the time to get from full value to the sustain level
* Sustain Level: steady state of key
* Release Time: the time to get from sustain level to zero

The shape of envelope

* switch: first attack, first release
* swell in: increase attack time
* fade out: increase release time
* damped pluck/ strike(hit sound): first attack, some decay, zero sustain, zero release
* blowing or bowing: long sustain level
* quirk: first attack, little decay, long release.


## LFO (Low Frequency Oscillator)
It's like envelope, it controls the parameters of modules.  
The main uses of an LFO is to create vibrato effect(vibrato is a cyclic variation in pitch that's found in most musical performances).  

You can make the matrix of below three points.

* source of modulation: ex. LFO
* the destination of modulation: ex.VCO (voltage control oscillator)
* amount of modulation

LFO has parameters as below. (The frequency of LFO is below under the human hearing (0 ~ 20Hz), so we can't hear that.)  

* frequency
* wave form
 * sin
 * triangle
 * saw
 * square

