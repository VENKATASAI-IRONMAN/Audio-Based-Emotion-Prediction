# Audio-based Emotion Prediction

## Project Description
This project aims to predict emotions from audio data using deep learning techniques. We utilize two datasets, CREMA-D and TESS, to train and evaluate a Convolutional Neural Network (CNN) for classifying emotions based on speech.

## Installation & Requirements
To set up the project environment:

1. Clone the repository:
   ```
   git clone https://github.com/your-username/audio-emotion-prediction.git
   cd audio-emotion-prediction
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

For detailed package information, refer to `requirements.txt`.

## Dataset Details
- **CREMA-D**: 7,442 audio samples of emotional speech from 91 actors
- **TESS**: 2,800 audio samples of emotional speech from 2 actresses

Both datasets contain recordings of various emotions including anger, disgust, fear, happiness, sadness, and neutral states.

For more information, see `data/README.md`.

## Key Findings (EDA Summary)
- Balanced distribution of emotions in both datasets
- MFCC features show distinct patterns for different emotions
- Spectrograms and waveforms provide visual insights into emotional characteristics of speech

## How to Use the Notebook
1. Open `Audio-based-Emotion-Prediction.ipynb` in Jupyter Notebook or Google Colab
2. Ensure all required libraries are installed (see requirements.txt)
3. Run cells sequentially to:
   - Load and preprocess the data
   - Perform exploratory data analysis
   - Train the CNN model
   - Evaluate model performance

## Results & Visualizations
- The CNN model achieves high accuracy in emotion classification
- Visualizations include:
  - Waveforms and spectrograms of sample audio files
  - Training and validation accuracy/loss curves
  - Confusion matrix of model predictions

For detailed results, refer to `reports/README.md`.

## Future Enhancements
- Experiment with other deep learning architectures (LSTM, Transformer)
- Incorporate transfer learning from pre-trained audio models
- Develop a real-time emotion prediction system
- Explore multi-modal emotion recognition (combining audio with text or video)

## 🤝 Contributing
Feel free to fork this repository and submit pull requests if you have improvements or new insights to add.

## License
This project is open-source and available under the MIT License.