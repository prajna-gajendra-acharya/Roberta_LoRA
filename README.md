# RoBERTa LoRA Fine-Tuning for AG News Classification

This repository contains a parameter-efficient fine-tuning (PEFT) implementation using LoRA (Low-Rank Adaptation) on the `roberta-base` model for multi-class text classification on the AG News dataset.

## 🚀 Project Overview

We fine-tuned RoBERTa using LoRA adapters injected into the attention layers (query and value) while keeping most of the base model frozen. This approach significantly reduces the number of trainable parameters to under 1 million, making it ideal for low-resource environments.

## 📊 Results (Best Epoch)

- **Accuracy**: 93.28%
- **Precision**: 93.46%
- **Recall**: 93.38%
- **F1 Score**: 93.42%
- **Trainable Parameters**: ~815K
- **LoRA Config**: `r=6`, `alpha=24`, `dropout=0.05`

## 📁 Files and Structure

- `Final_Results/` – Contains the best model checkpoint, tokenizer, training configs, and adapter files.
- `*.ipynb` – Colab notebook with training code, hyperparameter sweeps, evaluation, and visualizations.
- `README.md` – Project summary and setup instructions.
