# Deep Learning Applications Labs

This repository contains the implementation of three lab projects for the **Deep Learning Applications** exam.

---

## Table of Contents

* [Project Overview](#project-overview)
* [Lab Summaries & Setup](#lab-summaries--setup)
    * [Lab 1: CNNs](#lab-1-cnns)
    * [Lab 3: Transformers](#lab-3-transformers)
    * [Lab 4: OOD Detection](#lab-4-ood-detection)
* [General Instructions for Running Labs](#general-instructions-for-running-labs)
* [Contributing](#contributing)

---

## Project Overview

This repository serves as a practical exploration of key deep learning topics. It includes **Jupyter Notebooks** and associated files for reproducing experiments and understanding the underlying principles. The labs are designed to be self-contained, allowing for focused learning on specific areas of deep learning.

---

## Lab Summaries & Setup

Below you'll find a brief description of each completed lab and the specific instructions to set up the necessary environment and run the notebooks.

### Lab 1: CNNs

**Description:**
In this first laboratory, you'll gain practical experience working with Deep Models, particularly **Convolutional Neural Networks (CNNs)**, in sophisticated ways. We'll reproduce (on a small scale) the results of the Residual Networks paper, demonstrating that deeper doesn't always mean better. Subsequent exercises will ask you to delve deeper into the inner workings of CNNs.

**Key Paper:**
* **Deep Residual Learning for Image Recognition** by Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun. (arXiv:1512.03385)

**Setup & Running:**
To get started with Lab 1, recreate an Anaconda environment suitable for this lab using the following command:

```bash
conda create -n DLA -c conda-forge jupyterlab ipython matplotlib scikit-learn tqdm pytorch torchvision tensorboard standard-imghdr
```
Once the environment is created, activate it and launch the Jupyter Notebook for the lab:
```bash
conda activate DLA
jupyter lab Lab1-CNNs.ipynb
```
---

### Lab 3: Transformers

**Description:**
In this third laboratory session, we'll learn how to work with the **HuggingFace** ecosystem to adapt pre-trained models to new tasks. As you'll see, much of what's required is investigation into the inner workings of the HuggingFace abstractions. With a little work and trial-and-error, it's fairly easy to get a working adaptation pipeline up and running.

**Key Paper:**
* **Attention Is All You Need** by Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser, and Illia Polosukhin. (arXiv:1706.03762)

**Setup & Running:**
For this lab, you'll need a conda environment with the following packages:

```bash
conda create -n 'transformers' -c conda-forge transformers datasets matplotlib scikit-learn torchvision pytorch-gpu accelerate sentencepiece jupyterlab ipywidgets tqdm
```

After creating the environment, activate it and then open the Jupyter Notebook:

```bash
conda activate transformers
jupyter lab Lab3-Transformers.ipynb
```
---

### Lab 4: OOD Detection

**Description:**
In this laboratory session, we'll develop a methodology for detecting **Out-of-Distribution (OOD)** samples and measuring the quality of OOD detection. We'll also experiment with incorporating adversarial examples during training to render models more robust to adversarial attacks.

**Key Paper:**
* **A Simple Unified Framework for Detecting Out-of-Distribution Samples and Adversarial Examples** by Kimin Lee, Kibok Lee, Honglak Lee, and Jinwoo Shin. (arXiv:1706.02690)

**Setup & Running:**
For Lab 4, you can use the same **transformers** conda environment set up for Lab 3, as its dependencies are generally sufficient for this lab.

```bash
conda activate transformers
```

Then, launch Jupyter Lab and open the relevant notebook:

```bash
jupyter lab Lab4-OOD.ipynb # Or the specific notebook name within the Lab4-OOD directory
```
---

## General Instructions for Running Labs

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    cd your-repository-name
    ```
2.  **Navigate to the Lab Directory:**
    Each lab has its own directory (e.g., `Lab1-CNNs/`, `Lab3-Transformers/`, `Lab4-OOD/`). Navigate to the specific lab you want to run.
3.  **Create and Activate Conda Environment:**
    Follow the `conda create` command provided for each specific lab to set up its dedicated environment. Then, activate it:
    ```bash
    conda activate your-environment-name
    ```
4.  **Launch Jupyter Lab:**
    Once your environment is active, launch Jupyter Lab and open the relevant notebook:
    ```bash
    jupyter lab YourLabNotebook.ipynb
    ```
5.  **Run the Notebook:**
    Execute the cells within the Jupyter Notebook to explore the code and see the results.

---

## Contributing

For deeper understanding and troubleshooting, the following resources can be highly beneficial:

* **Gemini, ChatGPT:** For general questions about deep learning concepts, code snippets, or explanations.
* **Stack Overflow:** An excellent community resource for specific programming questions and error resolution.
* **Official Documentation:**
    * **PyTorch Documentation:** For detailed information on PyTorch's functionalities, layers, and operations.
    * **HuggingFace Transformers Documentation:** Essential for working with pre-trained models, tokenizers, and pipelines.
    * **NumPy Documentation:** For efficient numerical operations in Python.
    * **Matplotlib Documentation:** For data visualization.
    * **Scikit-learn Documentation:** For machine learning utilities and metrics.
