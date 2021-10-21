# OpenXTalk Apple AVAudioSampler
An OXT Builder Module that binds to Apple's AudioUnit Sampler Synth!

https://www.youtube.com/watch?v=va9WbnLrc00

Version 0.1:

Proof of concept working on macOS, yeah!

- Loads Apple's General MIDI Soundbank (gs_instruments.dls from inside the CoreAudio bundle).

Note On & Note Off Messages

Version 0.2:

Loads DLS & SF2 from files on the fly with program change and bank selecting

Version 0.3:
- Loads DLS & SF2 from files on the fly with program change and bank selecting
- Loads EXS24 (Logic/GarageBand sampler instruments) & Apple Sampler .AUPresets files

Version 0.4:

- Loads loose Sound Files (mp3,aiff,wav,etc.) files*
  *this handler seems to crash quite a bit when loading more sounds, memory management issue.

Version 0.5

- Loads loose Sound Files (mp3,aiff,wav,etc.) files
  *Temp fix for problem loading individual audio files(s) turns out it was a bug in LiveCode Builder
  should be fixed in the next LC Release.
- Added a few functions to get info on state of the Audio Engine & AUSampler

Version 0.6

- Added AUSampler global settings: Gain, Stereo Pan, Tuning

Version 0.6.5 ish:
- Added Pitchbend Send
- Added General MIDI Controller Send
- Bug Fixes & Minor or Cosmetic Updates to Demo Stack
- Demo stack now has button that scans for EXS Instruments from GarageBand & Logic standard Sampler Instruments folders

Version 0.7:

- Added inline documentation
- Changed some handler names, and parameters, updated demo stack for changes.
- Added some parameter checking
- Added MIDI Data Grid demo (which should work with AVAudioSampler, CoreMIDI, or AVMIDIPlayer on macOS (as well as built-in MIDI Player on Windows and Android platforms)
