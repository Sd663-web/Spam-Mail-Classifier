# 📧 Spam Mail Detection using Machine Learning

A Machine Learning project that detects whether an email/message is **Spam** or **Not Spam (Ham)** using **Logistic Regression**.

The project demonstrates a complete Machine Learning workflow — from data preprocessing and text feature extraction to model training, evaluation, and prediction.

---

## 🚀 Project Overview

Spam emails are unwanted messages that may contain advertisements, scams, malicious links, or other irrelevant content.

This project uses **Natural Language Processing (NLP)** and **Logistic Regression** to automatically classify messages into two categories:

* 🟢 **Ham** — Legitimate / non-spam message
* 🔴 **Spam** — Unwanted or suspicious message

The model learns patterns from previously labelled messages and uses those patterns to classify new messages.

---

## 🧠 Machine Learning Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Text Preprocessing
   ↓
Feature Extraction
   ↓
Train-Test Split
   ↓
Logistic Regression
   ↓
Model Evaluation
   ↓
Spam / Ham Prediction
```

---

## 🛠️ Technologies Used

| Technology              | Purpose                       |
| ----------------------- | ----------------------------- |
| 🐍 Python               | Programming Language          |
| 🧮 Pandas               | Data Manipulation             |
| 🔢 NumPy                | Numerical Computation         |
| 📊 Matplotlib / Seaborn | Data Visualization            |
| 🤖 Scikit-learn         | Machine Learning              |
| 📝 NLP                  | Text Processing               |
| 📈 Logistic Regression  | Classification Algorithm      |
| 📓 Jupyter Notebook     | Development & Experimentation |

---

## 📂 Project Structure

```text
Spam-Mail-Detection/
│
├── dataset/
│   └── spam.csv
│
├── notebooks/
│   └── spam_detection.ipynb
│
├── src/
│   └── spam_detection.py
│
├── models/
│   └── spam_model.pkl
│
├── requirements.txt
├── README.md
└── .gitignore
```

> The exact folder structure can be modified according to your project files.

---

## 📊 Dataset

The model is trained on a labelled dataset containing messages classified as:

* `spam`
* `ham`

Each record contains a text message along with its corresponding class label.

The dataset is processed before training to remove unnecessary information and convert the text into numerical features that can be understood by the Machine Learning algorithm.

---

## 🔄 Data Preprocessing

The following preprocessing steps are performed:

1. Loading the dataset
2. Removing unnecessary columns
3. Handling missing values
4. Removing duplicate records
5. Cleaning text data
6. Separating messages and labels
7. Converting text into numerical features
8. Splitting the dataset into training and testing sets

---

## 🔤 Feature Extraction

Machine Learning algorithms cannot directly process raw text.

Therefore, the text messages are converted into numerical vectors using a text feature extraction technique such as:

* **TF-IDF Vectorization**
* or **Count Vectorization**

For example:

```text
"Congratulations! You won a free prize"
```

is transformed into a numerical representation that the Logistic Regression model can process.

---

## 🤖 Machine Learning Model

### Logistic Regression

The primary classification algorithm used in this project is **Logistic Regression**.

Although its name contains "Regression", Logistic Regression is widely used for **binary classification problems**.

In this project:

```text
Spam     → 0
Ham      → 1
```

The model estimates the probability that a given message belongs to the spam class.

### Why Logistic Regression?

Logistic Regression is a good choice for text classification because:

* It is computationally efficient.
* It works well with high-dimensional text features.
* It is relatively easy to interpret.
* It provides probability-based predictions.
* It performs well for many binary classification tasks.

---

## 📈 Model Evaluation

The trained model can be evaluated using several classification metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

Example:

```text
Accuracy  : XX.XX%
Precision : XX.XX%
Recall    : XX.XX%
F1-Score  : XX.XX%
```

> Replace the `XX.XX%` values with the actual results obtained from your model.

### Confusion Matrix

The confusion matrix helps understand how many messages were correctly and incorrectly classified.

```text
                  Predicted
                Ham     Spam

Actual Ham      TN       FP
Actual Spam     FN       TP
```

---

## 🧪 Example Prediction

The trained model can be used to classify a new message.

### Input

```text
"Congratulations! You have won a free lottery ticket."
```

### Output

```text
Prediction: SPAM 🚨
```

Another example:

### Input

```text
"Hey, are we meeting at 5 PM today?"
```

### Output

```text
Prediction: HAM ✅
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Spam-Mail-Detection.git
```

### 2. Navigate to the Project

```bash
cd Spam-Mail-Detection
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

If your project uses a Python script:

```bash
python src/spam_detection.py
```

If you are using Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
notebooks/spam_detection.ipynb
```

and run the cells sequentially.

---

## 📦 Requirements

Example `requirements.txt`:

```text
numpy
pandas
scikit-learn
matplotlib
seaborn
jupyter
```

---

## 💡 Key Learning Outcomes

Through this project, I explored:

* Natural Language Processing
* Text preprocessing
* Feature extraction
* TF-IDF / Count Vectorization
* Binary classification
* Logistic Regression
* Train-Test Splitting
* Model evaluation
* Confusion Matrix
* Precision, Recall and F1-Score
* Building an end-to-end Machine Learning pipeline

---

## 🔮 Future Improvements

Some possible improvements include:

* [ ] Try Naive Bayes classification
* [ ] Compare Logistic Regression with SVM and Random Forest
* [ ] Perform hyperparameter tuning
* [ ] Improve NLP preprocessing
* [ ] Handle class imbalance
* [ ] Deploy the model using Flask or FastAPI
* [ ] Create a web interface for spam detection
* [ ] Add real-time email classification
* [ ] Deploy the application using Streamlit
* [ ] Improve model performance using advanced NLP techniques

---

## 📌 Conclusion

This project demonstrates how Machine Learning and Natural Language Processing can be combined to solve a real-world problem such as **spam message detection**.

Using text preprocessing, feature extraction, and Logistic Regression, the system can learn patterns from labelled messages and classify new messages as **Spam** or **Ham**.

---

## 👨‍💻 Author

**Soumyajit Dalal**

B.Tech — Computer Science & Engineering

Interested in:

* Machine Learning
* Data Science
* Software Development
* Web Development
* Artificial Intelligence

---

## ⭐ If You Like This Project

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub!

```text
⭐ Star this repository
🍴 Fork it
🐛 Report issues
💡 Suggest improvements
```
