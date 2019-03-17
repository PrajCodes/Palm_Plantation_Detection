# Palm_Plantation_Detection
My attempt at finetuning Pytorch pretrained models tp solve  Women in Data Science 2019 Datathon challenge 

WiDS Datathon is data focused hackathon and this years challenge was to detect the presence of palm plantations in satellite images. 
Problem statement : https://www.kaggle.com/c/widsdatathon2019

I have used Transfer Learning approach to look at this problem : i.e Feature extraction from the torchvision
models

Feature extraction means we start with a pretrained model (here, pytorch's face recognition model) and only update the final layer weights
from which we derive predictions. It is called feature extraction
because we use the pretrained CNN as a fixed feature-extractor, and only
change the output layer.

This model has achieved  0.992 Score based on  Area under ROC curve between the predicted probability and the observed target (wheather the image has oilpalm or not )

Further the IPython notebook attached has comments explaining each step to follow 

**Reference**
Using Transfer Learning :
Finetuning and Feature extraction from the `torchvision
models <https://pytorch.org/docs/stable/torchvision/models.html>`
