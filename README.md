# Fake News Detection Using BERT

This project is part of the Phase 2 report focusing on Fake News Detection using BERT (Bidirectional Encoder Representations from Transformers). The aim of this project is to leverage transformer-based models for classifying news articles as **fake** or **real** using the FNC-1 dataset.

---

## Project Structure

```
📂 Project Root
│
├── Model-Py.py                        # Main Python script for model implementation
├── Model-notebook.ipynb               # Jupyter Notebook for model experimentation
├── test_bodies.csv                    # CSV file containing test article bodies
├── train_bodies.csv                   # CSV file containing training article bodies
├── train_stances.csv                  # CSV file with stances for training articles
├── train_stances.random.csv           # Randomized version of the stance file
├── phase 2 project report.pdf         # Detailed project report for Phase 2
└── README.md                          # Project documentation
```

---

## Installation

To get started, clone the repository and install the necessary dependencies:

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available, install the following dependencies manually:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn transformers
```

Ensure you have Jupyter Notebook installed:

```bash
pip install notebook
```

---

## Usage

To run the main script:

```bash
python Model-Py.py
```

To launch the notebook:

```bash
jupyter notebook Model-notebook.ipynb
```

Follow the cells in order to replicate results and understand the analysis.

---

## Description

- `Model-Py.py`: Contains the core logic for data processing, model training, and evaluation using BERT. It handles the preprocessing of text, tokenization, fine-tuning, and prediction.

- `Model-notebook.ipynb`: Provides step-by-step visualization and analysis of the model, along with parameter tuning and evaluation. This notebook also includes SHAP explainability methods for better interpretation of the model's decision-making.

- `test_bodies.csv`: Contains the body of articles for testing the model.

- `train_bodies.csv`: Holds the body of articles for model training.

- `train_stances.csv`: Lists the stances for the corresponding training articles (e.g., agree, disagree, discuss, unrelated).

- `train_stances.random.csv`: A randomized version of the training stances to test model robustness.

- `phase 2 project report.pdf`: The full project report, including methodology, experiments, and findings related to fake news detection using BERT and Word2Vec models.

---

## Results

All outputs, visualizations, and performance metrics are displayed within the notebook. Key results include:

- Model accuracy
- Precision and recall metrics
- Visualizations of decision boundaries and confusion matrices
- SHAP interpretability plots for understanding word-level impact

---

## Dependencies

Make sure you have the following libraries installed:

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `transformers`
- `shap`

---

## Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

---

## License

This project is licensed under the MIT License.
