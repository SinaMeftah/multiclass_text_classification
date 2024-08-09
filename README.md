# Fine-Tuning LLM Models for Multi-class Text Classification

## Overview
This repository demonstrates a multi-class text classification analysis using the Hugging Face Transformers library. The project showcases how to perform sentiment analysis or any other multi-class text classification task by fine-tuning Large Language Models (LLMs) using different approaches.

## Dataset
The dataset used in this project is the Emotion Dataset by dair-ai (https://hf.co/datasets/emotion). It consists of English Twitter messages labeled with six basic emotions: anger, fear, joy, love, sadness, and surprise. The labels are of the ClassLabel type and are represented as integers. This dataset is suitable for training and evaluating text classification models that can recognize and categorize emotions expressed in text.

## Fine-Tuning Approach
This project employs a range of fine-tuning techniques to adapt LLMs to text classification tasks, including:

* Fine tuning whole model: Updating the pre-trained model weights adapting it to task at hand.
* Low-Rank Adaptation (LoRA): Adapting the pre-trained model using low-rank matrices to learn task-specific features, while keeping the original model weights frozen. This approach allows for efficient adaptation of large models with minimal additional parameters and far less GPU memory usage.

## Getting Started
To reproduce the results in this repository, follow these steps:

1. Clone the repository: git clone https://github.com/SinaMeftah/multiclass_text_classification.git
    * or: gh repo clone SinaMeftah/multiclass_text_classification
2. Install the required libraries: pip install -r requirements.txt
3. Run the notebook
    * Note: Running these notebooks requires a good GPU with sufficient memory (based on batch size and fine tuning approach). If you don't have access to a suitable GPU, we recommend running the notebooks on platforms like Kaggle or Google Colab. If you do have a suitable GPU, you can clone the repository and run the notebooks locally. Make sure to install the required libraries and dependencies before running the notebooks.

## Contributions
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request.
