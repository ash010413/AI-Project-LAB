# Speech Emotion Recognition

I built this project in 2022 as an undergraduate AI lab project. The goal was to
classify emotion from short speech recordings using audio features and a neural
network classifier.

The notebook extracts MFCC, chroma, and mel-spectrogram features with `librosa`,
then trains a scikit-learn `MLPClassifier` on selected emotions from the RAVDESS
speech dataset. The saved notebook records an accuracy of 70.83% on its test
split. A sample WAV file is included for the final prediction example.

## Running it

You will need Python, Jupyter, and the audio/ML dependencies used by the
notebook:

```sh
python3 -m venv .venv
source .venv/bin/activate
pip install jupyter librosa numpy scikit-learn soundfile pyaudio
jupyter lab
```

The full RAVDESS dataset is not included. Place it in a folder named
`speech-emotion-recognition-ravdess-data` beside the notebook, preserving its
`Actor_*` folder structure. PyAudio may also require PortAudio to be installed
on the system.

## Status

Archived undergraduate work. The notebook and dependencies date from 2022 and
may need small compatibility fixes. There is no deployed demo.
