# What do you want?

If my understanding of audio is correct, and that this turns out to be a real (albeit small) problem, then what do I want this project to lead to?

What good can possibly come out of this for the audio world at large?

## Detection

It must become easier to realize that this is actually a problem in an audio file. Should this be a feature of the DAW? An analyzer plugin? Separate software? I don't know.

What I do know is that I want to avoid this distortion when I do audio projects. And the first step on the road to avoiding it is to know that it happens in the first place. Once I get that alert, I can choose my approach. 

## Remediation

Ok, so we know the problem is in the audio. How do we fix? Reduce gain? Subtractive EQ? Multi-band compressor? Or a whole new type of tool? There seems to be many options, probably more than I can imagine.

### Reduce gain

I have tested this and it is an effective way to remove the distortion. But it comes with a pretty obvious side effect - the sound becomes less audible in the mix. 

Sound normalization is a version of gain manipulation that is usually based on the peak RMS of the audio. Could the same be done, but instead of peak RMS, it uses the peak at whatever frequency is loudest throughout the file? Technically it is no issue to do so, but it would still have the side effect of reducing the volume of the whole sound.

### Subtractive EQ

This is also an effective way to remove the problem, but it will change the sound. The offending frequencies will be reduced, while the surrounding frequencies are not. This could lead to an unnatural sound in theory. Is that really a problem?

### Multi-band compressor / targeted compressor

A compressor could reduce or remove this problem. It would need to know a threshold of where to start reducing the volume of certain bands/frequencies, and would more or less function the same as subtractive EQ as far as I can understand - except perhaps for some differences in handling dynamics.

### Frequency-sensitive limiter

The difference between compressors and limiters might make this point moot, but a frequency-sensitive limiter could stop any frequency from passing a set threshold, even if the RMS level for the sound itself is not near the threshold. Could also sound unnatural perhaps?
