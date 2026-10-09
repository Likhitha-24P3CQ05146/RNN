# Movie Review Sentiment Analysis Using RNN

## 📌 Overview

This project uses a Recurrent Neural Network (RNN) to classify IMDB movie reviews as **Positive** or **Negative**. It uses the built-in IMDB dataset provided by TensorFlow/Keras and a stacked SimpleRNN architecture to learn patterns in text sequences and predict sentiment.

## 🚀 Features

* Binary sentiment classification.
* Built-in IMDB movie review dataset.
* Text sequence padding for uniform input length.
* Stacked SimpleRNN layers for sequential learning.
* Dropout layers to help reduce overfitting.
* Model evaluation using test accuracy and loss.
* Sentiment prediction for unseen reviews.

## 🛠️ Technologies Used

* Python
* TensorFlow and Keras
* NumPy
* Recurrent Neural Network (RNN)
* SimpleRNN, Embedding, and Dense layers

## 🧠 Model Architecture

* **Vocabulary size:** 10,000 words
* **Maximum sequence length:** 200 words
* **Embedding dimension:** 64
* **RNN layers:** Two stacked SimpleRNN layers with 64 and 32 units
* **Dense layers:** 32 and 16 neurons with ReLU activation
* **Dropout:** 0.3
* **Output layer:** One neuron with sigmoid activation
* **Optimizer:** Adam
* **Loss function:** Binary Cross-Entropy
* **Training:** 5 epochs with a batch size of 64

## ⚙️ Installation

Clone the repository:

```bash
git clone <your-repository-url>
cd RNN-Sentiment-Analysis
```

Install the required libraries:

```bash
pip install tensorflow numpy
```

## ▶️ Usage

Run the Python script:

```bash
python sentiment_analysis.py
```

The program loads the IMDB dataset, preprocesses the reviews, builds and trains the RNN model, evaluates its performance, and predicts the sentiment of a test review.

## 📊 Output

The program displays:

* Number of training and testing samples.
* Shape of the padded training data.
* RNN model architecture and parameters.
* Training and validation metrics.
* Test loss and test accuracy.
* Predicted sentiment and actual sentiment for a sample review.

**Prediction labels:**

* `0` — Negative
* `1` — Positive

## 🔮 Future Improvements

* Experiment with LSTM and GRU architectures.
* Tune hyperparameters to improve performance.
* Add custom movie review input and prediction.
* Visualize training accuracy and loss.
* Save the trained model for reuse.

## ⚠️ Limitations

The model uses a limited vocabulary and fixed-length sequences. Its performance depends on training, preprocessing, and model configuration.
