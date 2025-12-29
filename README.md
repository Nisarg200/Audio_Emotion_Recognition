🎙️ Audio Emotion Recognition (SER)
📌 Overview

This project addresses the task of Speech Emotion Recognition (SER), which aims to detect and classify the emotional content of speech signals. The work is carried out as part of an academic assignment and follows the complete SER workflow, from data exploration to model evaluation and comparison.

🎯 Problem Statement

Build the best possible speech emotion recognition system using the given emotion-labeled speech dataset by:

Evaluating a zero-shot pretrained model

Training a domain-specific supervised model

Comparing methods using standard classification metrics

Discussing advantages and limitations of each approach

🗂️ Dataset

Emotion-labeled speech audio from multiple sources:

RAVDESS

CREMA-D

SAVEE

TESS

Emotions covered (7 classes):
Angry, Happy, Sad, Neutral, Fearful, Disgusted, Surprised

📎 Dataset link:
https://www.kaggle.com/datasets/uldisvalainis/audio-emotions/data

Audio files are in .wav format.
Train / Dev / Test splits are created manually as part of the notebook.

⚙️ Methodology & Pipeline
Task 1: Zero-Shot Emotion Recognition

Used a pretrained HuBERT-based model

No task-specific training performed

Direct emotion prediction via learned speech representations

Task 2: Supervised Emotion Classification

Extracted MFCC features from speech signals

Trained an SVM classifier with RBF kernel

Model trained and evaluated on domain-specific data

Common Steps

Audio loading and preprocessing

Feature extraction (MFCCs for supervised model)

Model inference / training

Performance evaluation and comparison

📊 Evaluation Metrics

Both approaches are compared using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

Classification Report

A detailed analysis is provided in the notebook and report.

🧠 Conclusion

HuBERT zero-shot evaluation demonstrates the strength of pretrained self-supervised speech models without domain adaptation

MFCC + SVM (RBF) provides a strong supervised baseline when trained on task-specific data

Each approach involves trade-offs between generalization, interpretability, and data dependency

This project highlights practical SER system design along with a clear comparison of zero-shot and supervised learning approaches.
