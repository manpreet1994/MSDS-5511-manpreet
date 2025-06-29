# Metastatic Cancer Detection (CNN & Vision Transformer)

This repository contains code for detecting metastatic cancer in small image patches using the PatchCamelyon (PCam) dataset. The project explores and compares the performance of both Convolutional Neural Network (CNN) and Vision Transformer (ViT) architectures for this binary classification task.

## Project Description

The primary goal is to develop an algorithm to accurately identify metastatic cancer in 96x96 digital pathology image patches. The solution implements a robust data pipeline using TensorFlow's `tf.data.Dataset` and Pillow for efficient image loading and preprocessing. It then trains and evaluates a custom CNN model and a Vision Transformer model, comparing their effectiveness for this specific medical imaging challenge.

## Installation

To set up the project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/manpreet1994/MSDS-5511-manpreet.git
    cd MSDS-5511-manpreet/week3
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install tensorflow pandas scikit-learn matplotlib Pillow
    ```
4.  **Download the dataset:**
    Obtain the PCam dataset images and `labels.csv` from Kaggle or another source. Place the images in a `data/` subdirectory within the `week3` folder, and ensure `labels.csv` is also in `week3/`.

## Usage

To train and evaluate the CNN model:

Run the notebook `week3_image_classification.ipynb`

## Results and Conclusion

In our experiments, the Convolutional Neural Network (CNN) generally demonstrated more efficient learning and comparable or superior performance for this task compared to the Vision Transformer (ViT). This is likely attributed to the CNN's inherent inductive biases (like locality and translation equivariance), which are highly advantageous for processing local features in image data and enable better generalization on datasets of this size.

## License

This project is licensed under the MIT License