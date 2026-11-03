# 📩 SMS Spam Classification using Deep Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/NLP-4B8BBE?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Deep%20Learning-FF6F00?style=for-the-badge" />
</p>

## 📌 Project Overview

This project focuses on building a Deep Learning-based SMS Spam Classification system using **Recurrent Neural Networks (RNNs)** and Natural Language Processing (NLP).

The main objective is to automatically classify SMS messages into two categories:

- **Spam (1):** Unwanted or fraudulent messages.
- **Ham (0):** Legitimate messages.

Four different recurrent neural network architectures were implemented and evaluated to compare their performance on the SMS classification task.

## 🎯 Project Objectives

- Apply Natural Language Processing techniques to text classification.
- Build a vocabulary from SMS messages.
- Convert text messages into numerical sequences.
- Implement different RNN-based architectures using PyTorch.
- Train and evaluate multiple Deep Learning models.
- Compare model performance using test accuracy.

## 📊 Dataset

The project uses the **SMS Spam Collection Dataset**, containing 5,574 SMS messages labeled as spam or legitimate.

**Dataset Source:** [SMS Spam Collection – Hugging Face](https://huggingface.co/datasets/ucirvine/sms_spam)

| Dataset Split | Number of Messages |
|---|---:|
| Training Set | 4,459 |
| Testing Set | 1,115 |
| Total | 5,574 |

The dataset was shuffled using a fixed random seed and divided into 80% training and 20% testing data.

## ⚙️ Methodology

The project follows these main steps:

**1. Text Processing**
- Convert messages to lowercase.
- Split messages into individual words.
- Build a vocabulary from the training data.
- Use special tokens for padding (`<PAD>`) and unknown words (`<UNK>`).

**2. Sequence Preparation**
- Convert text messages into numerical sequences.
- Apply padding to handle variable-length messages.
- Use PyTorch Dataset and DataLoader for efficient batch processing.

**3. Model Development**

Four recurrent neural network architectures were implemented:

| Architecture | Description |
|---|---|
| Vanilla RNN | Basic recurrent neural network |
| GRU | Gated Recurrent Unit |
| LSTM | Long Short-Term Memory |
| BiLSTM | Bidirectional LSTM |

**4. Model Training**
- Optimizer: Adam
- Loss Function: Cross Entropy Loss
- Learning Rate: 0.001
- Batch Size: 32
- Hidden Dimension: 128
- Training Epochs: 10

## 🧠 Model Performance

The four models were evaluated on the same held-out test set.

| Model | Test Accuracy |
|---|---:|
| Vanilla RNN | 97.76% |
| GRU | 98.21% |
| LSTM | 97.94% |
| **BiLSTM** | **98.48%** |

<details>
<summary>📈 View Model Comparison</summary>

BiLSTM achieved the highest test accuracy among the four implemented architectures, followed by GRU, LSTM, and Vanilla RNN.

</details>

## 🛠️ Technologies & Libraries

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=plotly&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</p>
## 📁 Repository Structure

```text
SMS-Spam-Classification/
│
├── README.md
│
└── Week_8_Solved_Notebook.ipynb
```

## 🚀 How to Run

**1. Clone the repository**

```bash
git clone https://github.com/mohamed3611/SMS-Spam-Classification.git
```

**2. Navigate to the project directory**

```bash
cd SMS-Spam-Classification
```

**3. Install the required libraries**

```bash
pip install numpy pandas matplotlib torch scikit-learn datasets
```

**4. Run the Notebook**

Open `Week_8_Solved_Notebook.ipynb` using Jupyter Notebook or Google Colab.

The dataset is loaded directly from Hugging Face, so an internet connection is required.

## 📚 Key Learnings

Through this project, I gained practical experience in:

- Working with sequential text data.
- Understanding recurrent neural network architectures.
- Implementing RNN, GRU, LSTM, and BiLSTM using PyTorch.
- Handling variable-length input sequences.
- Training and evaluating Deep Learning models.
- Comparing different neural network architectures.

---

## 👨‍💻 Author

**Mohamed Tamer**

Computer Science Student | Aspiring AI Engineer

- GitHub: [@mohamed3611](https://github.com/mohamed3611)
- LinkedIn: [Mohamed Tamer](https://www.linkedin.com/in/mohamed-tamer-27270837a/)
- Email: mohamedd.t.mamdouh@gmail.com

---

<p align="center">
  ⭐ If you find this project interesting, feel free to explore the repository!
</p>
