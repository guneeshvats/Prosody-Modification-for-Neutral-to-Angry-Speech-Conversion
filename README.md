# Prosody-Modification-for-Neutral-to-Angry-Speech-Conversion
<h3>What are the files in this repository :</h3> <br>

- `Phase_Vocode.ipynb` file: Phase Vocoder code in python.
- `neutral1`, `angry_speech1`: Sample input of neutral speech converted to teh angry speech.
- `works.png`: It is a block diagram of how the whole poject works.
- `Final_Report`: It is the complete report for our project.
- There are waveforms pngs also showing the changes observed in time domain.


Transforming neutral speech into an angry-sounding version. By leveraging signal processing techniques, we enhance the pitch and intensity characteristics typically associated with angry speech.
<br><br>
![How it works](https://github.com/guneeshvats/Prosody-Modification-for-Neutral-to-Angry-Speech-Conversion/assets/70188630/4f3457dc-d82b-4dca-898f-4e7ac8a6d4b8)
<br>
Our approach begins by dividing the speech signal into frames using windowing. We then separate the voiced and unvoiced parts of each frame, as only the voiced segments possess pitch and undergo most of the energy increase during angry speech. This separation is achieved using an energy threshold.
<br><br>
The voiced frames are processed using a phase vocoder, a powerful tool for modifying pitch and duration parameters. Through time-scaling and pitch-shifting functions, we increase the pitch and shorten the duration to emulate angry speech characteristics. The phase vocoder operates on smaller frames within each voiced frame, utilizing a Hanning window to minimize signal alteration caused by windowing effects.
<br><br>
<strong><em>In this repository, you will find a Python implementation of the phase vocoder, making use of libraries such as SciPy, Librosa, NumPy, Matplotlib, and OS. This code allows for practical exploration and experimentation with prosody modification in speech signal processing.</em></strong>
