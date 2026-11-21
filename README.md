# 🎬 IMDB Movie Reviews – Sentiment Analysis
### Comparative Study of Simple RNN, LSTM, and GRU

A Deep Learning project focused on **Sentiment Analysis** using the IMDB Movie Reviews dataset. The goal is to build, train, evaluate, and compare three Recurrent Neural Network architectures (RNN, LSTM, and GRU) to classify movie reviews as Positive or Negative.

---

## 📌 Project Overview

This project implements a complete NLP sentiment classification pipeline using TensorFlow and Keras.

It explores how different recurrent neural network architectures understand sequential text data and how their performance differs in terms of classification metrics and training time.

The project also includes real-world review predictions and error analysis to better understand model behavior.

## 🎯 Objectives

- Load and explore the IMDB movie reviews dataset.
- Preprocess text data using encoding and padding.
- Build and train three deep learning models:
  - Simple RNN
  - LSTM
  - GRU
- Evaluate models using multiple classification metrics.
- Compare model performance and training time.
- Predict sentiment for new movie reviews.
- Analyze incorrect predictions to understand model limitations.

## 🛠️ Technologies & Libraries

| Technology | Purpose |
|---|---|
| Python | Main Programming Language |
| TensorFlow / Keras | Deep Learning Model Development |
| NumPy | Numerical Operations |
| Pandas | Data Manipulation |
| Matplotlib | Data Visualization |
| Scikit-learn | Model Evaluation |
| Regular Expressions (re) | Text Processing |
| Jupyter Notebook | Development Environment |

## 📂 Dataset

**IMDB Movie Reviews Dataset**

The dataset is provided by Keras and contains:

- 50,000 movie reviews.
- 25,000 training samples.
- 25,000 testing samples.
- Binary sentiment labels:
  - `0` → Negative
  - `1` → Positive

The reviews are represented as integer-encoded sequences using a predefined vocabulary.

## ⚙️ Project Workflow

### 1. Data Preparation
- Import required libraries.
- Configure model and training parameters.
- Load the IMDB dataset.
- Explore encoded and decoded reviews.
- Analyze review length distribution.
- Decode reviews into readable text.
- Apply padding and truncation to ensure fixed-length sequences.

### 2. Simple RNN
- Build an Embedding layer.
- Add a SimpleRNN layer.
- Apply Dropout for regularization.
- Use a Sigmoid output layer for binary classification.
- Train and evaluate the model.
- Visualize confusion matrix and learning curves.

### 3. LSTM & GRU
Build and train two additional models using the same general architecture, replacing the recurrent layer with LSTM and GRU.

Evaluate both models using the same evaluation pipeline.

### 4. Model Comparison
Compare all three architectures using:

- Accuracy
- Precision
- Recall
- F1 Score
- Training Time

Visualize the results using separate bar charts to identify the best-performing and fastest models.

### 5. Real Predictions
Test the trained models using new movie reviews.

The prediction pipeline includes:
- Text cleaning and tokenization.
- Word-to-integer encoding.
- Handling unknown and out-of-vocabulary words.
- Padding sequences.
- Predicting sentiment and confidence.

### 6. Error Analysis
- Identify incorrectly classified test samples.
- Compare predicted labels with actual labels.
- Decode and display misclassified reviews.
- Investigate possible reasons behind incorrect predictions.

## 🧠 Model Architectures

| Model | Description |
|---|---|
| Simple RNN | Processes sequential information using recurrent connections. |
| LSTM | Uses memory cells and gates to capture long-term dependencies. |
| GRU | Uses update and reset gates with a simpler architecture than LSTM. |

All three models use an Embedding layer, Dropout regularization, and a Sigmoid output layer.

## 🔧 Configuration

The main hyperparameters used in this project:

| Parameter | Value |
|---|---:|
| Vocabulary Size | 10,000 |
| Maximum Review Length | 200 |
| Embedding Dimension | 128 |
| RNN Units | 64 |
| Batch Size | 64 |
| Maximum Epochs | 10 |
| Random State | 42 |
| Optimizer | Adam |
| Loss Function | Binary Crossentropy |
| Early Stopping Patience | 2 |

## 📊 Evaluation Metrics

The models are evaluated using:

- **Accuracy:** Measures the overall percentage of correct predictions.
- **Precision:** Measures how many predicted positive reviews are actually positive.
- **Recall:** Measures how many actual positive reviews are correctly identified.
- **F1 Score:** Combines Precision and Recall into a single metric.
- **Training Time:** Measures the time required to train each model.

## 🚀 Installation & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

### 2. Navigate to the Project Directory

```bash
cd YOUR_REPOSITORY
```

### 3. Install Dependencies

```bash
pip install numpy pandas matplotlib tensorflow scikit-learn jupyter
```

### 4. Run Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and execute all cells sequentially from top to bottom.

**Note:** Training time depends on your hardware. Running all three models may take some time, especially without GPU acceleration.

## 📈 Expected Results

After training, the notebook generates:

- Individual evaluation reports for RNN, LSTM, and GRU.
- Confusion matrices for all models.
- Training and validation accuracy curves.
- Training and validation loss curves.
- A comprehensive model comparison table.
- Performance comparison charts.
- Predictions on new movie reviews.
- Examples of incorrectly classified reviews.

Actual results may vary depending on hardware and training conditions.

## 💡 Key Learning Outcomes

Through this project, I gained practical experience in:

- Natural Language Processing (NLP).
- Text preprocessing and sequence encoding.
- Word Embeddings.
- Recurrent Neural Networks.
- Understanding the differences between RNN, LSTM, and GRU.
- Deep Learning model training and evaluation.
- Performance comparison and visualization.
- Real-world sentiment prediction.
- Error analysis and model interpretation.

## 👨‍💻 Author

**Marwan Tamer**

AI & Machine Learning Engineer | AI & Data Science Student

- GitHub: [@marwanTamer](https://github.com/marwanTamer)

---

⭐ If you find this project useful, feel free to explore the repository!
