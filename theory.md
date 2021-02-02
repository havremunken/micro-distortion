# Theory

Again, I am new at audio, and would in no way dare call myself an engineer. I lack the skills and the vocabulary. Therefore, if you find something wrong in the text, my understanding, or anything on this page, please let me know so I can try to fix it.

## Clipping as used in audio language today refers only to RMS

My understanding is that RMS is calculated as a mean across time and frequency spectrum.

The true peak of the Windows 10 audio file in question is calculated to be in the -8.4 to -8.5dBFS range. It is never even close to clipping.

However, a small PART of the frequency spectrum (approximately 200-600Hz) DOES contain energy levels that creep above 0dBFS.

These areas are so small that they are not enough to "raise" the average RMS level above the threshold. But they still cross it, and the result is partial distortion of that frequency range - at least on my [equipment](equipment.md). 

## You need fairly good speakers to be able to hear this

Windows 10 is running on what - billions of machines? At least quite a few. The gear I have connected is probably slightly above the average PC speaker setup, but compared to actual audio studio gear, it would be low-end. However, most people would not hear this sound on equipment with accurate enough audio reproduction that the distortion would be audible.

The alternative here is of course that there is something wrong with my setup.

## Lowering the audio level in software removes the distortion

If I use subtractive EQ on the 200-600Hz region, OR if I reduce the gain of the audio file so that no part of the frequency spectrum ever crosses the 0dBFS threshold, the distortion is gone. I can play the file as loud as I want (volume levels where it is painful to be in the room), and there is no sign of distortion. This would seem to me to take care of the following objections:

- My setup is faulty and causing me to hear distortions.
- The audio file was recorded "too hot".

If it was recorded too hot, wouldn't that have "flattened" the sound/waveform in the offending frequencies? Keep in mind I lack the tools to see only the 200-600Hz section of the frequency spectrum as a waveform so this assumption might be faulty.

## The average sound pressure level (RMS) is not the only thing that could clip/distort

As I believe this project shows, defending against clipping is not just about keeping RMS levels below 0dBFS. We also need tools that can warn and help us when parts of the spectrum go above digital zero - for more on this, see [What do you want?](whatdoyouwant.md).
