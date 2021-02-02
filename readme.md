# Micro-distortion in audio - research project

This project is an attempt to document something I discovered while working on an audio project. It is probably known to real audio engineers, but I have not yet been able to find much material about it online, or found that this phenomenon is known by a name. I am calling it micro-distortion until I discover what it is actually called.

## What is this about?

### TL;DR version

Energy levels in parts of the frequency spectrum that go above 0dBFS, but the RMS of the total waveform does NOT cross 0dBFS and this is thus apparently not considered "clipping".

### Slightly more elaborate version

While working on an audio project, I discovered distortion in the audio - kind of like clipping - where there should be none. The RMS level peaked at -17dBFS or so according to Adobe Audition. Yet the distortion was there and noticeable, every time. I looked closer at the file and saw that the waveform as drawn by Audition indeed peaked out around -17dBFS. I then added an equalizer and saw what I believe to be the issue - even though the RMS level is well below 0dBFS, there were certain frequencies where the energy level actually did cross 0dBFS. In the time dimension, these incidents corresponded exactly with the distortion I was hearing.

I also know I hear this distortion from time to time, and one instance of this is something most of us that work with Windows 10 will have heard many times. The "Asterisk" sound file, specifically `C:\Windows\Media\Windows Background.wav`, also has this problem on my system. I repeated the process and found the same issue here, which I consider extremely helpful, as this is a file that will be easy to get a hold of for many people and it isn't just something I produced by mistake.

Unless anything else is specified, all testing is performed using this file from Windows 10.

## Questions and findings

These are the major questions and findings I have written up to this point. I have tried to organize these into separate files in a way that makes sense, in part also to avoid the wall of text this would otherwise quickly become.

- [Equipment used for testing](equipment.md)
- [Detecting and measuring the problem](measuring.md)
- [My feeble attempt at a theory](theory.md)
- [How to contribute to this project](contributing.md)
- [What do I hope to accomplish with this project](whatdoyouwant.md)

I am trying to keep an open mind without the brain falling out, so suggestions are very welcome!

## Disclaimers

I am not an audio engineer. I am not a researcher. I do not believe I have discovered something that nobody else ever knew about. I am just trying to learn about how digital audio works, and also find answers to all the questions raised by my trivial finding.

I am trying to use the correct terminology, but as I am new at this, I will probably be fairly ignorant. If you find a wrong use of terminology, or an opportunity to improve things, raising and issue or creating a pull request would be most welcome. Or you can contact me and inform me using one of the contact methods I will eventually remember to provide.