# README

## Website
[Birdcall Classification Using Deep Learning](https://rahulchhatbar.github.io/Birdcall-Classification-Using-Deep-Learning/)

## Dataset
[Cornell Birdcall Identification](https://www.kaggle.com/competitions/birdsong-recognition/data)

## Overview
Initially, the dataset comprises over 21,000 audio files spanning 264 classes. However, upon conducting Exploratory Data Analysis (EDA), it became evident that the audio files were not uniform in several aspects. Firstly, we observed that the number of audio files present for each class are not equal in terms of audio duration and the duration mentioned in the file for each file was not. Also, the file format of audio files was not constant; there were audio files present in other formats (wav, wma, etc). To address these issues, a filtering process was implemented. Classes were selected where the total duration of data files fell between 3000 and 4500 minutes, and files shorter than 3 seconds were filtered out. We had 40 classes after filtering out.

## Instructions

### For Data Preparation

Step 1: Execute `audio_selection.ipynb` which will create a dataset for 40 classes.

### For ResNet

Step 2: Execute `preprocessing.ipynb` to preprocess the data and generate Mel spectrograms which are used to train our models.

Step 3: Execute code for ResNet50 in `ResNet50.ipynb`.

### For YAMNet

Step 2: Execute `preprocessing.ipynb` to preprocess the data and generate Mel spectrograms which are used to train our models.

Step 3: Execute code for YAMNet in `YAMNet.py`.

### For EfficientNet

A distinct preprocessing approach was devised which will generate spectrogram images for every 5 seconds of the audio data. Hence the input for the EfficientNet originates after executing Step 1.

Step 2: Execute code for EfficientNet in `EfficientNet.ipynb`.
