## CS316 Data Science and AI Project

An AI-powered system that identifies famous Quran reciters and detects which Surah and Ayah is being recited from audio recordings.

## 🎯 Features

- *Reciter Identification*: Achieves 100% accuracy in identifying reciters using ECAPA-TDNN speaker embeddings
- *Verse Detection*: Automatic Arabic speech-to-text transcription using Whisper
- *Text Matching*: Multi-strategy fuzzy matching to identify exact Surah and Ayah
- *Interactive UI*: User-friendly Gradio interface for testing

## 📊 Dataset

- *Audio Files*: 22 Surah recordings from 4 famous reciters
  - Abdul Basit Abdul Samad
  - Mishary Al-Afasy
  - Abdulrahman Al-Sudais
  - Islam Sobhi
- *Text Data*: Complete Quran text (6,236 verses) in Arabic

## 🛠️ Technologies Used

- *Python 3.8+*
- *SpeechBrain*: Speaker recognition (ECAPA-TDNN)
- *OpenAI Whisper*: Arabic speech-to-text
- *Scikit-learn*: Classification models
- *Librosa*: Audio feature extraction
- *Gradio*: Web interface

## 📦 Installation

1. Clone the repository:
bash
git clone https://github.com/YOUR_USERNAME/CS316_Quran_Reciter_Project.git
cd CS316_Quran_Reciter_Project


2. Create virtual environment:
bash
python -m venv venv
venv\Scripts\activate  # Windows


3. Install dependencies:
bash
pip install -r requirements.txt


## 🚀 Usage

1. Open Jupyter Notebook or Google Colab
2. Load notebooks/quran_reciter_analysis.ipynb
3. Run all cells sequentially
4. The Gradio interface will launch automatically

## 📈 Model Performance

| Component | Metric | Score |
|-----------|--------|-------|
| Reciter Classification | Accuracy | 100% |
| Reciter Classification | F1-Score | 1.00 |
| Verse Detection | Top-3 Accuracy | ~90% |
| Text Matching | Similarity | 85-95% |

## 📁 Project Structure

CS316_Quran_Reciter_Project/
├── notebooks/
│   └── quran_reciter_analysis.ipynb    # Main analysis notebook
├── data/
│   ├── quran_full.csv                   # Complete Quran text
│   └── audio/                           # Recitation audio files
│       ├── abdulbasit_abdulsamad/
│       ├── mishary_al_afasy/
│       ├── abdulrahman_sudias/
│       └── islam_sobhi/
├── models/
│   ├── embeddings_db.pkl                # Cached embeddings
│   ├── reciter_classifier.pkl           # Trained classifier
│   └── (other model files)
├── requirements.txt                     # Python dependencies
├── README.md                            # This file
├── .gitignore                          # Git ignore rules
└── LICENSE                             # Project license


## Methodology

### 1. Data Collection & EDA
- Audio quality analysis
- Duration distribution
- Reciter statistics
- Feature visualization

### 2. Feature Engineering
- ECAPA-TDNN speaker embeddings
- MFCC acoustic features
- Arabic text normalization

### 3. Model Training
- Speaker recognition using SpeechBrain
- Logistic Regression for reciter classification
- Whisper for Arabic transcription
- Fuzzy text matching for verse identification

### 4. Evaluation
- Confusion matrices
- Precision, Recall, F1-Score
- Cross-validation results

## 📋 Project Requirements (CS316 Checklist)

- ✅ Exploratory Data Analysis (EDA)
- ✅ Data cleaning and preprocessing
- ✅ Feature engineering
- ✅ Visualization (histograms, bar charts, heatmaps)
- ✅ Machine Learning models (Classification)
- ✅ Model evaluation metrics
- ✅ Model comparison
- ✅ Interactive UI (Gradio)
