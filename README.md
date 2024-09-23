# Prosody Modification: Neutral to Angry Speech Conversion

A project to transform neutral speech into an angry-sounding version using prosody modification techniques. By leveraging signal processing, we enhance the pitch and intensity characteristics typically associated with angry speech.

---

## 📂 Repository Overview

- **`Phase_Vocode.ipynb`**: Python implementation of the Phase Vocoder.
- **`neutral1`, `angry_speech1`**: Sample input/output files (neutral and angry speech).
- **`works.png`**: Block diagram explaining the project workflow.
- **`Final_Report`**: Complete project report.
- **Waveform PNGs**: Visual representations showing time-domain changes.

---

## 🔧 How It Works

<img src="https://github.com/guneeshvats/Prosody-Modification-for-Neutral-to-Angry-Speech-Conversion/assets/70188630/4f3457dc-d82b-4dca-898f-4e7ac8a6d4b8" alt="How it works" width="500"/>

Our approach involves:

1. **Frame Division**: We divide the speech signal into frames using windowing.
2. **Voiced/Unvoiced Separation**: Voiced frames are identified using an energy threshold, as these contain pitch and most of the energy increase during angry speech.
3. **Phase Vocoder**: Voiced frames undergo pitch and duration modification through time-scaling and pitch-shifting using the phase vocoder.
4. **Pitch Enhancement**: Pitch is increased and the duration is shortened to emulate angry speech characteristics.

The phase vocoder operates on smaller subframes, utilizing a Hanning window to minimize distortion.

---

## 🛠️ Tools & Libraries

- **SciPy**
- **Librosa**
- **NumPy**
- **Matplotlib**
- **OS**

---

## 📁 Folder Structure

```bash
Prosody-Modification-for-Neutral-to-Angry-Speech-Conversion/
│
├── Phase_Vocode.ipynb         # Phase Vocoder implementation in Python
├── Final_Report.pdf           # Complete project report
├── works.png                  # Block diagram of the workflow
├── neutral1.wav               # Sample neutral speech file
├── angry_speech1.wav          # Sample angry speech file
├── waveforms/                 # Directory containing waveform PNGs
│   ├── waveform1.png
│   └── waveform2.png
└── README.md                  # Project overview and documentation
```
---

This repository provides a hands-on Python implementation to explore prosody modification in speech signal processing.

