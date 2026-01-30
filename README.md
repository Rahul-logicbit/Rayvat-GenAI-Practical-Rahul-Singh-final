# Rayvat-GenAI-Practical-Rahul-Singh-final
Submission for Rayvat Outsourcing Generative AI Practical Test (via Jenya Platform). LSTM text generator trained on Shakespeare's works.
# Shakespeare Language Model (LSTM)

## Project Overview
This repository contains a Generative AI solution designed to replicate the writing style of William Shakespeare. It was developed as part of the technical assessment for **Jenya / Rayvat Outsourcing**.

The solution implements a **Stacked LSTM (Long Short-Term Memory)** neural network using TensorFlow/Keras to predict and generate text sequences.

## Key Features (Addressing Evaluation Criteria)
* **Architecture (Creativity):** Implements a **2-layer Stacked LSTM** with Dropout regularization (0.2) to capture deeper linguistic patterns and prevent overfitting.
* **Sampling Strategy (Problem Solving):** Uses **Temperature Sampling** during generation rather than simple Argmax. This allows tunable creativity:
    * *Low Temperature (0.2)*: Predictable, grammatically strict.
    * *High Temperature (0.8)*: Creative, diverse vocabulary usage.
* **Code Quality:** Fully Object-Oriented (OOP) implementation with type hinting, docstrings, and modular design.

## Technical Details
| Component | Specification |
| :--- | :--- |
| **Framework** | TensorFlow 2.x / Keras |
| **Embedding** | 100-dimension vector space |
| **Hidden Layers** | 2x LSTM (256 units each) |
| **Optimization** | Adam Optimizer (LR=0.001) |
| **Dataset** | [Tiny Shakespeare (Karpathy)](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt) |

## How to Run
1. Open the provided Jupyter Notebook `Jenya_GenAI_Task_Rahul_Singh.ipynb`.
2. Ensure GPU runtime is enabled (if using Colab).
3. Run all cells sequentially.
