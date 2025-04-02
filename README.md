# Book Recommendation System

A deep learning-based collaborative filtering recommendation system for books using the Book-Crossing dataset. This system predicts user ratings for books based on both user and book features.

## Overview

This project implements a neural network-based recommendation system that:
- Uses collaborative filtering to predict book ratings
- Incorporates both user and book features
- Provides personalized book recommendations
- Achieves good prediction accuracy on the test set

## Features

- User embedding layer for learning user preferences
- Item embedding layer for learning book characteristics
- Dot product layer for rating prediction
- Regularization to prevent overfitting
- Data preprocessing and feature engineering
- Model evaluation and recommendation generation

## Dataset

The model uses the Book-Crossing dataset from Kaggle, which contains:
- Book information (ISBN, title, author, year of publication, publisher)
- User information (user ID, location, age)
- Rating information (user ratings for books)

## Setup

1. Clone the repository:
```bash
git clone <repo-url>
cd book-recommendation-system
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Place the dataset files in the `data` directory:
- BX_Books.csv
- BX-Users.csv
- BX-Book-Ratings.csv

## Usage

1. Run the Jupyter notebook:
```bash
jupyter notebook model.ipynb
```

2. Execute all cells in sequence to:
- Load and preprocess the data
- Train the model
- Generate recommendations

## Model Architecture

The recommendation system uses a neural network with:
- User embedding layer (256 → 128 → 32 neurons)
- Item embedding layer (256 → 128 → 32 neurons)
- Dot product layer for rating prediction
- L2 normalization for embeddings

## Performance

The model achieves:
- Training loss: ~0.56
- Test loss: ~0.57
- Efficient training on 66,003 samples
- Good generalization on test set

## Author

Philip Titus

## Connect with Me

- 🌐 [Personal Website](https://mrphilip.pythonanywhere.com/)
- 🛍️ [Shop](https://pmart-pi.vercel.app/)
- 👥 [LinkedIn](https://linkedin.com/in/philiptitus)

## License

Copyright © 2025 Philip Titus. All rights reserved. 