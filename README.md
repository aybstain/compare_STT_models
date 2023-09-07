# Speech Recognition and Evaluation

This repository contains code for performing speech recognition using various speech-to-text (STT) engines and evaluating the results. The following STT engines are covered in this repository:

- Google Speech Recognition (GSR)
- IBM Watson STT
- Whisper
- Vosk
- Wav2Vec2
- WavLM
- SpeechT5

## Evaluation Metrics

### Word Error Rate (WER)

Word Error Rate (WER) is a common metric used to evaluate the performance of speech recognition systems. It measures the dissimilarity between the recognized text and the ground truth (reference) text. WER calculates the number of word substitutions, insertions, and deletions needed to transform the recognized text into the reference text, normalized by the total number of words in the reference text.

In this project, we calculate WER to assess the accuracy of various speech-to-text (STT) models. Lower WER values indicate better recognition accuracy.

### Character Error Rate (CER)

Character Error Rate (CER) is another important metric for evaluating STT models. It measures the dissimilarity between the recognized text and the reference text at the character level. Similar to WER, CER quantifies the number of character substitutions, insertions, and deletions required to align the recognized text with the reference text, normalized by the total number of characters in the reference text.

CER provides a finer-grained evaluation of recognition accuracy, especially for applications where character-level accuracy is critical.

### Latency

Latency refers to the time delay between inputting an audio signal and receiving the corresponding recognized text output. In our project, we measure latency to evaluate the real-time performance of different STT models. Lower latency values indicate faster recognition and response times, which are crucial in applications where low latency is a requirement.

## Data Source

The audio data used in this project was sourced from the LibriSpeech dataset. LibriSpeech is a widely used dataset for speech recognition research and contains a diverse collection of English-language audio recordings from audiobooks. The dataset is split into various subsets, including train, dev (development), and test sets, making it suitable for training and evaluating speech recognition models.

By using LibriSpeech data, we ensure that our evaluation is based on a standardized and publicly available dataset, allowing for fair comparisons between different STT models.

We got 12 audios for each 9 users.

These evaluation metrics (WER, CER, and latency) and the use of the LibriSpeech dataset help us objectively assess and compare the performance of various STT engines, allowing us to make informed decisions about their suitability for specific applications.

## Results 

<img width="667" alt="Capture (1)" src="https://github.com/aybstain/compare_STT_models/assets/103702856/7f5d077e-72a8-44b2-bd91-61f1f3e01971">

<img width="665" alt="Capture1 (1)" src="https://github.com/aybstain/compare_STT_models/assets/103702856/ff771414-0985-4a7f-b3e2-1fb7170cf26a">

![download (3)](https://github.com/aybstain/compare_STT_models/assets/103702856/5597ff9b-e87b-4720-977b-051715cfd4c9)

Other visualizations can be seen in the code.


