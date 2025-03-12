# Audio-based Emotion Prediction Dataset

## Dataset Overview
This project uses two datasets for audio-based emotion prediction:

1. CREMA-D (Crowd-sourced Emotional Multimodal Actors Dataset)
2. TESS (Toronto Emotional Speech Set)

## CREMA-D Dataset
- **Source**: https://github.com/CheyneyComputerScience/CREMA-D
- **Description**: Audio-visual dataset of facial and vocal emotional expressions
- **File Format**: WAV
- **Emotions**: Anger, Disgust, Fear, Happy, Neutral, Sad
- **Sample Count**: 7,442 clips from 91 actors

### Data Columns
1. **Emotions**: Categorical (angry, disgust, fear, happy, sad, neutral)
2. **Path**: String (file path to the audio file)

## TESS Dataset
- **Source**: https://tspace.library.utoronto.ca/handle/1807/24487
- **Description**: Set of 200 target words spoken in the carrier phrase "Say the word _____" by two actresses (aged 26 and 64 years)
- **File Format**: WAV
- **Emotions**: Anger, Disgust, Fear, Happy, Pleasant Surprise, Sad, Neutral
- **Sample Count**: 2,800 files (200 target words × 7 emotions × 2 actresses)

### Data Columns
1. **Emotions**: Categorical (angry, disgust, fear, happy, neutral, ps, sad)
2. **Path**: String (file path to the audio file)

## Usage
1. Load the datasets using pandas:
   ```
   import pandas as pd
   
   crema_df = pd.read_csv('path_to_crema_csv')
   tess_df = pd.read_csv('path_to_tess_csv')
   ```

2. Access audio files using the 'Path' column in each dataframe.

3. Use librosa to load and process audio files:
   ```
   import librosa
   
   audio, sr = librosa.load(file_path)
   ```

## Data Preprocessing
- Extract features like MFCC, chroma, mel, contrast, and tonnetz from audio files.
- Normalize features using StandardScaler.
- Encode emotion labels using LabelEncoder or OneHotEncoder.

## Note
Ensure you have the necessary permissions and follow the dataset's usage guidelines when using these datasets for your project.