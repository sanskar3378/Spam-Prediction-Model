# Spam Prediction Model

## Project Title & Overview

Spam Prediction Model is a machine learning project designed to classify SMS-style messages as either spam or legitimate (ham). The project demonstrates how text classification works in practice using a Naive Bayes classifier, one of the most effective and widely used algorithms for text-based classification tasks.

The notebook in this repository covers the entire machine learning workflow:
- loading a labeled dataset
- preprocessing message text
- converting text into numerical features
- training a classifier
- evaluating predictions
- testing the model on new messages

## Repository Structure

```text
Spam-Prediction-Model/
├── LICENSE
├── README.md
├── data/
│   └── spam.csv
├── notebooks/
│   └── model.ipynb
└── requirements.txt
```

### Files Included
- `data/spam.csv`: the dataset used for training and evaluation
- `notebooks/model.ipynb`: the notebook containing the full analysis, preprocessing, feature extraction, model training, and prediction steps
- `README.md`: project documentation and setup steps
- `requirements.txt`: Python dependencies needed to run the project

## Prerequisites

Before running the project, ensure the following are installed:

- Python 3.9 or later
- Jupyter Notebook or JupyterLab
- pip package manager

Required packages:
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

## Installation

1. Clone the repository:

```bash
git clone https://github.com/sanskar3378/Spam-Prediction-Model.git
cd Spam-Prediction-Model
```

2. Create and activate a virtual environment:

```bash
python -m venv venv
```

On macOS/Linux:
```bash
source venv/bin/activate
```

On Windows:
```bash
venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available yet, install manually:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib jupyter
```

## Usage Guide

1. Place the dataset file into the `data/` folder:
   - Example: `data/spam.csv`

2. Open the notebook:

```bash
jupyter notebook notebooks/model.ipynb
```

3. Run all cells in order.

The notebook will:
- load the dataset
- clean and preprocess the text
- encode text into feature vectors
- train a Multinomial Naive Bayes model
- evaluate accuracy and classification metrics
- predict labels for new sample messages

## Model Overview

This project uses:
- `CountVectorizer` to transform text into numerical features
- `MultinomialNB` as the classifier for spam detection

The result is a fast and effective model for identifying spam messages from text input.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
