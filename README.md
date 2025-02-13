# Image-Classification
Image Classification on CIFAR-10   🛫 🚘 🐦 🐱 🦌 🐶 🐸 🐴 🚢 🛻

Information before starting
In this problem, we will explore different deep learning architectures for image classification on the CIFAR-10 dataset. Make sure that you are familiar with torch Tensors, two-dimensional convolutions (nn.Conv2d) and fully-connected layers (nn.Linear), ReLU non-linearities (F.relu), pooling (nn.MaxPool2d), and tensor reshaping (view). Make sure to read through all instructions in both this notebook and in the PDF while completing this problem!

Copying this Colab Notebook to your Google Drive
Since the course staff is the author of this notebook, you cannot make any lasting changes to it. You should make a copy of it to your Google Drive by clicking File -> Save a Copy in Drive.

Problem Introduction
You've already had some practice using the PyTorch library in HW3, but this problem dives into training more complex deep learning models.

The specific task we are trying to solve in this problem is image classification. We're using a common dataset called CIFAR-10 which has 60,000 images separated into 10 classes:

airplane
automobile
bird
cat
deer
dog
frog
horse
ship
truck
We've provided an end-to-end example of loading data, training a model, and performing evaluation. We recommend using this code as a template for your implementations of the more complex models. Feel free to modify or reuse any of the functions we provide.

Unlike other coding problems in the past, this one does not include an autograded component.

Enabling GPU
We are using Google Colab because it has free GPU runtimes available. GPUs can accelerate training times for this problem by 10-100x when compared to using CPU. To use the GPU runtime on Colab, make sure to enable the runtime by going to Runtime -> Change runtime type -> Select T4 GPU under "Hardware accelerator".

Note that GPU runtimes are limited on Colab. We recommend limiting your training to short-running jobs (under 15 minutes each) and spread your work over time, if possible. Colab will limit your usage of GPU time, so plan ahead and be prepared to take breaks during training. If you have used up your quota for GPU, check back in a day or so to be able to enable GPU again.

Your code will still run on CPU, so if you are just starting to implement your code or have been GPU limited by Colab, you can still make changes and run your code - it will just be quite a bit slower. You can also choose to download your notebook and run locally if you have a personal GPU or have a faster CPU than the one Colab provides. If you choose to do this, you may need to install the packages that this notebook depends on to your cse446 conda environment or to another Python environment of your choice.

To check if you have enabled GPU, run the following cell. If device is cuda, it means that GPU has been enabled successfully.
