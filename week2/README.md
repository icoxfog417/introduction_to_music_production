# Week2

## DAW
DAW is Digital Audio Workstation. It is used in "post-production".

* pre-production: Songwriting, Rehersal
* production: Performance and recording
* post-production: Mixing, Editing, Mastering


## DAW setting

* Audio device (in/out)
* Sample rate: 48000
* Bit depth: 24
* Buffer Size: 128 or 1024 (number of samples when digital to analog)
* File type: broadcast wav -> uncompressed/interleave 

Sample rate is samples per second. High sample rate takes more sample, so you can deal with high frequency sound.  
The frequency that human being can hear is about 20000, and you can use half of it. So generally sample rate is around 40000.  
(CD's sample rate is 44100).

Each sample is converted to 0/1 data that computer can understand. The length of data is bit depth (in other words "word").  
If relates to amplitude. So if bit depth is large, you can deal with loud sound. CD's bit depth is 16.

Buffer size is buffer for computer processing. Low buffer size means low latency, but you needs computer power (CPU, RAW),
and you can't use so many plugins.

File type relates to compression way, lossy or not. ZIP is not lossy but MP3 is.
Stereo sound cause left and right sound. So there are two files for one sound, interleaved file is contains both in single file.

Major tools

* Pro Tool
* Digital Performer 
* Abelton

[...and more](https://share.coursera.org/wiki/index.php/Musicproduction:daw)


## DAW project checklist

* Proper project name and location
* Digital audio preference (sample rate, bit depth ...)
* Recording file type
* Hardware settings
* Buffer size (start from 128, and up if necessary)

## Type of track

* Audio track: mono/stereo
* MIDI: like real time score. so used to send data to an external synthesizer
* Auxiliary(Aux) track: used primarily routing audio with a DAW
* Instrumental track: realize MIDI. receive MIDI and perform it　(inputs one type of data but outputs another).
* Global track: contain song specific information like Markers and Temp

most of the time, recording is mono track.

1. check your setting (ex. project setting, audio preference)
2. create a track (remember mono or stereo, depend on you input)
3. name the track
4. record enable the track
5. set levels using the microphone pre-amp
6. enable the click and countoff
7. record

## MIDI

**Channel**
MIDI has 1-16 channel. It's like TV channel, MIDI can use 16 difference instruments.  
ex. channel1 is piano, 2 is guitar ...

**Message**
To send/receive data, MIDI use "message".  
There are various type of message.

* Channel message: data to one of the channels
** channel voice: note of/off, velocity, ...
** channel mode: to set the channel status (Omni/mono/poly mode)...
* System message: 
** system common
** system real-time
** system exclusive

* synthesizer: create sound
* sampler: playback real sound

Synthesizer makes sound by calculating formula, so it needs CPU power.  
Sampler is just playing (recorded) audio file, so it doesn't need CPU power. But to store the many audio files, it needs disk volume.

