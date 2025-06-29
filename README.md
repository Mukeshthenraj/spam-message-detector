# Spam Message Detector

A Python project that classifies SMS text messages as spam or not spam using several machine learning models. The project demonstrates preprocessing, feature extraction, and model evaluation on a real dataset of messages.

## 🚀 Project Overview

This project explores different approaches to detect spam messages, including:

- **Count Vectorization** and **TF-IDF Vectorization** of text data.
- Extraction of additional features like:
  - Message length
  - Number of digits
  - Number of non-word characters
- Training multiple classifiers:
  - Multinomial Naive Bayes
  - Support Vector Machine (SVM)
  - Logistic Regression
- Evaluating models using **ROC AUC scores**.

By combining classic text processing with engineered features, the models achieve high performance in spam detection.

---

## 📂 Project Structure

```
.
├── LICENSE
├── README.md
├── spam.csv
└── spam_detector.py
```

- **LICENSE**: MIT License.
- **README.md**: Project description and usage.
- **spam.csv**: Dataset of labeled SMS messages.
- **spam_detector.py**: Main script containing all preprocessing and model training functions.

---

## 📊 Dataset

The dataset (`spam.csv`) includes SMS text messages labeled as:

- `spam`: Messages intended for advertising, fraud, or phishing.
- `ham`: Regular messages.

Each row contains:

- `text`: The message content.
- `target`: Label (1 = spam, 0 = not spam).

---

## ⚙️ Requirements

To run this project, install the following Python libraries:

```bash
pip install pandas numpy scikit-learn
```

---

## 🧩 How to Run

1. Clone the repository or download the files.
2. Make sure `spam.csv` and `spam_detector.py` are in the same folder.
3. Run the script:

```bash
python spam_detector.py
```

Each function (`answer_one()` to `answer_eleven()`) can be called to see the results of different analysis steps and models.

---

## 📈 Example Outputs

- **Percentage of spam messages:** ~13%
- **Longest token in vocabulary:** `"com1win150ppmx3age16subscription"`
- **Naive Bayes AUC Score:** ~0.99
- **SVM AUC Score:** ~0.99
- **Logistic Regression AUC Score:** ~0.99

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

This project was inspired by classic text classification techniques and demonstrates how combining vectorized features with engineered metadata can improve spam detection performance.

Feel free to use and adapt it in your own projects!

