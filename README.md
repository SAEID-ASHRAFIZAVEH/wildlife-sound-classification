# 🐾 Wildlife Sound Classification

A machine learning project that classifies wildlife animal sounds using the ESC-50 dataset and Random Forest algorithm.

## 📋 Project Overview

This project uses audio signal processing and machine learning to identify 12 different wildlife animal sounds including dogs, cats, birds, frogs, and farm animals. The model extracts MFCC (Mel-Frequency Cepstral Coefficients) features from audio files and uses a Random Forest classifier to predict the animal category.

## 🎯 Features

- **12 Wildlife Categories**: dog, rooster, pig, cow, frog, cat, hen, insects, sheep, crow, chirping_birds, crickets
- **Audio Feature Extraction**: MFCC features using librosa
- **Random Forest Classifier**: 100 estimators with optimized parameters
- **Comprehensive Evaluation**: Detailed classification report and confusion matrix visualization
- **Sample Testing**: Random sample predictions with accuracy metrics

## 📊 Results

- **Test Accuracy**: ~XX% (depends on your run)
- **Training Samples**: ~480 audio files
- **Testing Samples**: ~120 audio files
- **Feature Dimensions**: 40 MFCC coefficients

## 🛠️ Technologies Used

- **Python 3.x**
- **librosa**: Audio processing and feature extraction
- **scikit-learn**: Machine learning (Random Forest)
- **pandas**: Data manipulation
- **numpy**: Numerical operations
- **matplotlib & seaborn**: Data visualization
- **tqdm**: Progress bars

## 📁 Project Structure

```
wildlife-sound-classification/
│
├── wildlife_classification.py    # Main classification script
├── README.md                      # Project documentation
├── requirements.txt               # Python dependencies
├── .gitignore                    # Git ignore file
│
├── dataset/                      # Dataset folder (not included in repo)
│   ├── meta/
│   │   └── esc50.csv
│   └── audio/
│       └── *.wav files
│
└── results/                      # Output folder
    └── confusion_matrix.png
```

## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/wildlife-sound-classification.git
   cd wildlife-sound-classification
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the ESC-50 dataset**
   - Visit: [ESC-50 Dataset](https://github.com/karolpiczak/ESC-50)
   - Download and extract to a folder named `dataset`
   - Ensure the structure matches:
     ```
     dataset/
     ├── meta/
     │   └── esc50.csv
     └── audio/
         └── [2000 .wav files]
     ```

### Usage

1. **Update the dataset path** in `wildlife_classification.py`:
   ```python
   DATASET_PATH = r'C:\Users\YourName\path\to\dataset'
   ```

2. **Run the classification script**:
   ```bash
   python wildlife_classification.py
   ```

3. **View results**:
   - Check console output for accuracy metrics
   - Find confusion matrix saved as `confusion_matrix.png`

## 📈 How It Works

1. **Data Loading**: Reads ESC-50 metadata and filters wildlife categories
2. **Feature Extraction**: Extracts 40 MFCC coefficients from each audio file
3. **Train/Test Split**: Uses fold 5 for testing, folds 1-4 for training
4. **Model Training**: Trains Random Forest classifier with 100 trees
5. **Evaluation**: Generates accuracy metrics, classification report, and confusion matrix
6. **Sample Testing**: Tests on random samples with visual feedback

## 🎓 Learning Outcomes

- Audio signal processing with librosa
- Feature extraction for audio classification
- Machine learning with Random Forest
- Model evaluation and performance metrics
- Data visualization with matplotlib and seaborn

## 📝 Dataset Information

This project uses the **ESC-50 dataset**:
- **Source**: [ESC-50: Dataset for Environmental Sound Classification](https://github.com/karolpiczak/ESC-50)
- **Citation**: K. J. Piczak. ESC: Dataset for Environmental Sound Classification. Proceedings of the 23rd Annual ACM Conference on Multimedia, Brisbane, Australia, 2015.
- **License**: Creative Commons Attribution Non-Commercial

## 🔮 Future Improvements

- [ ] Add deep learning models (CNN, RNN)
- [ ] Implement data augmentation
- [ ] Add real-time audio classification
- [ ] Create web interface for predictions
- [ ] Experiment with other audio features (spectrograms, chromagrams)
- [ ] Cross-validation for more robust evaluation

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Saeid Ashrafizaveh**
- GitHub: https://github.com/SAEID-ASHRAFIZAVEH
- LinkedIn: www.linkedin.com/in/saeid-ashrafizaveh-839820291

## 🙏 Acknowledgments

- ESC-50 dataset creators
- librosa library developers
- scikit-learn community

---

⭐ If you found this project helpful, please consider giving it a star!