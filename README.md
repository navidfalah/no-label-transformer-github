# 🐍 GitHub No-Label Transformer

## 📝 Description
This Python script processes GitHub issue data, applies label transformations, and performs various NLP tasks using transformers and machine learning models. It includes data preprocessing, label mapping, text augmentation, and evaluation of models like Naive Bayes and Zero-Shot Classification. 🛠️

---

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/github-no-label-transformer.git
   cd github-no-label-transformer
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Install additional libraries:
   ```bash
   pip install git+https://github.com/scikit-multilearn/scikit-multilearn.git
   pip install datasets
   pip install nlpaug
   ```

---

## 🚀 Usage

1. Run the script:
   ```bash
   python github_no_label_transformer.py
   ```

2. The script will:
   - Load GitHub issue data from a URL.
   - Preprocess and transform labels.
   - Perform text augmentation.
   - Train and evaluate models (Naive Bayes, Zero-Shot Classification).
   - Visualize results using matplotlib.

---

## 📂 File Structure

```
github-no-label-transformer/
├── github_no_label_transformer.py  # Main script
├── README.md                       # This file
├── requirements.txt                # Dependencies
└── data/                           # (Optional) Data folder for local datasets
```

---

## 🧩 Key Features

- **Data Preprocessing**:
  - Load GitHub issues from a JSON dataset.
  - Map and filter labels for consistency.
  - Remove duplicates and handle missing data.

- **Text Augmentation**:
  - Use `nlpaug` to augment text data for better model training.

- **Model Training & Evaluation**:
  - Train a **Naive Bayes** model for multi-label classification.
  - Perform **Zero-Shot Classification** using Hugging Face transformers.
  - Evaluate models using **Micro** and **Macro F1 scores**.

- **Visualization**:
  - Plot word distributions, F1 scores, and other metrics using `matplotlib`.

---

## 📊 Example Outputs

1. **Label Distribution**:
   ```plaintext
   Number of labels: X
   Top-8 label categories:
   - tokenization: Y
   - new model: Z
   ```

2. **Model Performance**:
   - Micro F1 scores for Naive Bayes and Zero-Shot models.
   - Macro F1 scores for different thresholds and top-k values.

3. **Visualizations**:
   - Histogram of words per issue.
   - F1 score plots for different training sample sizes.

---

## 🤖 Models Used

- **Naive Bayes**: A simple yet effective model for multi-label classification.
- **Zero-Shot Classification**: Leverages Hugging Face transformers for label prediction without explicit training.
- **Text Augmentation**: Uses `nlpaug` to generate synthetic training data.

---

## 📈 Performance Metrics

- **Micro F1 Score**: Evaluates overall model performance across all labels.
- **Macro F1 Score**: Evaluates model performance for each label independently.

---

## 🛠️ Dependencies

- Python 3.x
- Libraries:
  - `pandas`, `numpy`, `matplotlib`
  - `scikit-learn`, `scikit-multilearn`
  - `datasets`, `transformers`, `nlpaug`
  - `torch` (for PyTorch-based models)

---

## 🤝 Contributing

Contributions are welcome! 🎉 Feel free to open an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature`.
3. Commit your changes: `git commit -m "Add your feature"`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a pull request.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Hugging Face for the `transformers` library.
- `nlpaug` for text augmentation.
- Google Colab for the initial notebook environment.

---

Enjoy coding! 🚀✨

--- 
