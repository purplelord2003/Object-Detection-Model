# Object Detection Model (Trash Detector)
### Deployed app demo: https://huggingface.co/spaces/purplelord2003/Trash_Object_Detector

#### Since we have already built image classification models in the [`PyTorch-Bootcamp`](https://github.com/purplelord2003/PyTorch-Bootcamp) repository, I will now be attempting to build an Object Detection Model using PyTorch. This model will attempt to detect trash objects in images.

#### This repository contains all the work I have done in the 2 Jupyter Notebooks in the `Jupyter Notebooks` folder. Do download the Jupyter Notebook's raw file to fix the formatting within the individual cells (the preview compresses the lines together) or open them in Google Colab using the links below. The `Demo preparation` folder contains the zip file that was then uploaded to Hugging Face spaces.

Notebook 1 (training model):
<a target="_blank" href="https://colab.research.google.com/github/purplelord2003/Object-Detection-Model/blob/main/Jupyter%20Notebooks/Trash_Object_Detection_Model.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Notebook 2 (deploying model):
<a target="_blank" href="https://colab.research.google.com/github/purplelord2003/Object-Detection-Model/blob/main/Jupyter%20Notebooks/Trash_Object_Detection_Model_Deployment.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## Summary
I attempted to train a pre-trained [Faster R-CNN model](https://pytorch.org/vision/stable/models/faster_rcnn.html) from PyTorch on the trash dataset. During the first run, an overfitting trend was quickly observed after a few epochs, leading to the validation loss being much higher than the training loss (resulting in an early stoppage). I attempted to fix this by introducing greater data augmentation such as random photometric distortion and random horizontal flip during the second run, yet this led to a model that performed slightly worse than the first run. Nevertheless, I chose the best performing model and deployed a Gradio demo in Hugging Face spaces. 
