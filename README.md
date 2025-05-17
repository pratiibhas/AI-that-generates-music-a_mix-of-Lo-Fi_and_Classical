# AI-that-generates-music-a_mix-of-Lo-Fi_and_Classical
 ## Overview
This project aims to build an AI system capable of generating music by learning from two distinct genres — Lo-Fi and Classical. The current progress covers data understanding, collection, and preparation.


## What is Audio data?
By nature, a sound wave is a continuous signal, meaning it contains an infinite number of signal values in a given time. This poses problems for digital devices which expect finite arrays. To be processed, stored, and transmitted by digital devices, the continuous sound wave needs to be converted into a series of discrete values, known as a digital representation.
The analog signal is first captured by a microphone, which converts the sound waves into an electrical signal. The electrical signal is then digitized by an Analog-to-Digital Converter to get the digital representation through sampling.

### some terms related to audio data
1. Sampling : Sampling is the process of measuring the value of a continuous signal at fixed time steps. The sampled waveform is discrete, since it contains a finite number of signal values at uniform intervals.
2. Amplitude : The amplitude of a sound describes the sound pressure level at any given instant and is measured in decibels (dB). We perceive the amplitude as loudness.
3. Audio as A Waveform :You may have seen sounds visualized as a waveform, which plots the sample values over time and illustrates the changes in the sound’s amplitude. This is also known as the time domain representation of sound.
4. The frequency spectrum :Another way to visualize audio data is to plot the frequency spectrum of an audio signal, also known as the frequency domain representation. The spectrum is computed using the discrete Fourier transform or DFT. It describes the individual frequencies that make up the signal and how strong they are.
5. Spectrogram :What if we want to see how the frequencies in an audio signal change? The problem is that the spectrum only shows a frozen snapshot of the frequencies at a given instant. The solution is to take multiple DFTs, each covering only a small slice of time, and stack the resulting spectra together into a spectrogram.
6. Mel Spectogram :A mel spectrogram is a variation of the spectrogram that is commonly used in speech processing and machine learning tasks. It is similar to a spectrogram in that it shows the frequency content of an audio signal over time, but on a different frequency axis.

# Data Pipeline
### Data Collection
   Downloaded lo-fi and Classical music and converted to mp3 file using python libraries. The audio files are arounf 6 hours of Lo-Fi audio and 6-7 hours of classical music audio.

### Data Preparation
1. Dissected long audio clips in 30 second .wav files.
2. Padded 0s to the ones which were less than 30 seconds.
3. The files were clean so there was no need to clear noise form the files.
