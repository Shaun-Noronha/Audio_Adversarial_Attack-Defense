# Audio Adversarial Attack and Defence
This is an implementation of an audio adversarial attack on the DeepSpeech Automatic Speech Recognition (ASR) system. The goal of this project is to generate adversarial audio samples that can cause the ASR system to misinterpret the original audio incorrectly or as the target transcription while maintaining perceptual similarity to the original audio.

This project utilizes the DeepSpeech ASR model, TensorFlow, and various signal processing techniques to craft adversarial perturbations for speech signals. It is essential to use this project responsibly and only for research and testing purposes with proper authorization.

## Features
* Untargeted and Targeted adversarial attack on the DeepSpeech ASR system
* Optimization loop to find adversarial perturbations
* Spectrogram and signal processing techniques
* Support for custom target transcriptions

## Usage
1. Download the DeepSpeech pre-trained models and scorer file:
   - Download [deepspeech-0.9.3-models.pbmm](https://github.com/mozilla/DeepSpeech/releases/download/v0.9.3/deepspeech-0.9.3-models.pbmm)
   - Download [deepspeech-0.9.3-models.scorer](https://github.com/mozilla/DeepSpeech/releases/download/v0.9.3/deepspeech-0.9.3-models.scorer)

2. Prepare the original audio file:
   * Replace 'normal0.wav' with your own audio file in WAV format. Ensure the audio sample rate is 16000 Hz.

3. Customize the target transcription:
   * Modify the target variable to set your desired target transcription.

4. Specify the number of iterations:
   * The attack will run for a specified number of iterations to find the adversarial perturbation that satisfies the target transcription.

## Results
The generated adversarial audio file will be saved as your desired filename. You can listen to the generated audio and check if it indeed causes the ASR system to produce the target transcription.

## Note
This project is intended for research purposes only and should be used responsibly. Unauthorized use of adversarial techniques may have harmful consequences. Always obtain proper authorization before testing adversarial attacks on any system.

## Acknowledgments
This project is based on the DeepSpeech ASR system by Mozilla - https://github.com/mozilla/DeepSpeech.

## Team Members
* Melita Lewis
* Sushree Nadiminty
* Angeica Sebastian
* Shaun Noronha

