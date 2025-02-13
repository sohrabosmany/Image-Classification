# Image Classification on CIFAR-10  

🚀🛫 🚘 🐦 🐱 🦌 🐶 🐸 🐴 🚢 🛻

## Overview
This project explores different deep learning architectures for **image classification** on the **CIFAR-10** dataset using **PyTorch**. The dataset consists of **60,000 images** categorized into **10 different classes**:

- ✈️ Airplane
- 🚗 Automobile
- 🐦 Bird
- 🐱 Cat
- 🦌 Deer
- 🐶 Dog
- 🐸 Frog
- 🐴 Horse
- 🚢 Ship
- 🛻 Truck

We provide an **end-to-end implementation** of loading data, training models, and evaluating performance, with templates for building and improving classification models.

---

## 🔧 Prerequisites
### Before You Start
To successfully complete this project, ensure you are familiar with the following **PyTorch** concepts:
- **Tensors**
- **Convolutional layers** (`nn.Conv2d`)
- **Fully-connected layers** (`nn.Linear`)
- **ReLU activations** (`F.relu`)
- **Pooling layers** (`nn.MaxPool2d`)
- **Tensor reshaping** (`view`)

### 📌 Cloning and Running the Notebook
Since the original notebook is read-only, **make a copy** in your Google Drive:
1. Open the notebook in **Google Colab**.
2. Click **File** → **Save a Copy in Drive**.

Alternatively, you can clone this repository and run the code locally:
```bash
# Clone the repository
git clone https://github.com/sohrabosmany/image-classification.git
cd image-classification

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter notebook
jupyter notebook image-classification.ipynb
```

---

## 📌 Problem Introduction
This project builds on **HW3**, where you were introduced to **PyTorch**. Now, we train **deeper models** for image classification using **CIFAR-10**. Our goal is to classify images into one of **10 categories** using neural networks.

Key steps:
1. Load and preprocess the **CIFAR-10** dataset.
2. Train **baseline and advanced deep learning models**.
3. Evaluate and fine-tune models.
4. Compare performance across architectures.

---

## ⚡ Enabling GPU Acceleration
To speed up training, **enable GPU** in Google Colab:
1. Go to **Runtime** → **Change runtime type**.
2. Select **T4 GPU** under **Hardware Accelerator**.
3. Click **Save**.

To check if GPU is enabled, run:
```python
import torch
print(torch.cuda.is_available())  # Should return True if GPU is active
```
⚠️ **Note**: Google Colab has a **limited GPU quota**. If you exceed usage limits, you may have to wait before accessing GPUs again.

---

## 📂 Dataset and Model Implementation
The **CIFAR-10** dataset is automatically downloaded when running the script. We provide an end-to-end **training pipeline** with:
- Data **loading** and **augmentation**.
- **CNN architecture** for classification.
- Training with **cross-entropy loss** and **Adam optimizer**.
- Model **evaluation** and performance metrics.

🔹 Feel free to modify and improve the architecture! 🔹

---

## 🚀 Running the Training
To start training, simply run:
```python
python train.py
```
Modify **hyperparameters** (e.g., learning rate, batch size) in `config.py`.

---

## 📊 Evaluation and Results
After training, evaluate the model with:
```python
python evaluate.py
```

Performance metrics include:
- **Accuracy** per class
- **Confusion matrix**
- **Loss curves**

---

## 🛠️ Contributing
Contributions are welcome! If you'd like to improve this project:
1. **Fork** the repository.
2. Create a **feature branch**.
3. Submit a **pull request**.

---

## 📜 License
This project is licensed under the **MIT License**.

Happy coding! 🎉
