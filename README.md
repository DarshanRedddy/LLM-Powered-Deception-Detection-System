**LLM-Powered-Deception-Detection-System**


Humans are not very good at telling when someone is lying, and human accuracy in detecting deception is very constrained.
This project explores the fine-tuning of MiniLM and other Large Language Models (LLMs) for deception and lie detection, evaluating their efficacy in discerning truthful versus deceptive statements.

About

This repository contains code and documentation for an LLM-powered deception detection system, leveraging MiniLM with two approaches:

Transfer Learning

Parameter-Efficient Fine-Tuning with LoRA

The goal is to assess the potential of LLMs in binary classification tasks like deception detection and demonstrate how modern NLP methods can outperform human baselines in lie detection accuracy.

Getting Started

Follow these steps to set up and run the project locally. Ensure you have the necessary dependencies installed.

Prerequisites

Python (>=3.6)

CUDA Environment (for GPU acceleration)

Required Python Packages

pandas (>=0.25.0)

numpy (>=1.18.0)

torch (>=1.0.0)

sentencepiece (>=0.1.0)

transformers (>=4.0.0)

datasets (>=1.1.0)

peft (>=1.0.0)

wandb (>=0.10.0)

scikit-learn (>=0.22.0)



Project Structure
<details> <summary>Directory Layout</summary>
LLM-Powered-Deception-Detection-System/
│── data/
│    └── Dataset.csv
│── notebooks/
│    └── Transfer_learning.ipynb
│── src/
│    ├── load_model.py
│    ├── main_LoRA.py
│    └── train.py
│── Fine_Tuning_of_MiniLM_Fin_report.pdf
│── MiniLM_Fine_tuning_presentation.pdf
│── README.md
│── requirements.txt

</details>
Files

Dataset.csv – Dataset for lie detection.

Fine_Tuning_of_MiniLM_Fin_report.pdf – Report describing methodology and results.

MiniLM_Fine_tuning_presentation.pdf – Presentation slides.

Transfer_learning.ipynb – Jupyter notebook for transfer learning experiments.

load_model.py – Utility for loading pretrained MiniLM.

main_LoRA.py – Implementation of LoRA fine-tuning.

train.py – Core training script.

Results

The system treats deception detection as a binary classification problem.
By fine-tuning MiniLM, the project achieved up to 70% accuracy, surpassing human baseline performance on the same task.

This shows that LLM-based fine-tuning can capture nuanced patterns in deceptive versus truthful text, highlighting the promise of LLM-powered deception detection systems for real-world applications.
