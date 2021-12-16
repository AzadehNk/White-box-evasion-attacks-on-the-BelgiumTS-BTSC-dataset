# White-box-evasion-attacks-on-the-BelgiumTS-BTSC-dataset
 Applying four white-box evasion attacks against two deep learning classification models on the BelgiumTS (BTSC) dataset.

This is the code fo four white-box evasion attacks against two deep learning classification models on the BelgiumTS (BTSC) dataset. In this project we used VGG16 and ResNet50 deep-learning classification models, and implemented Fast Gradient Sign Method (FGSM), Projected Gradient Descent (PGD), DeepFool attack, and Carlini & Wagner l2 as white-box evasion attacks against the above deep learning models.

## Data
This project is used [Belgium traffic sign classification (BTSC)](https://btsd.ethz.ch/shareddata/) dataset which is a subset of the Belgium traffic sign dataset. This dataset involves 62 classes with 4591 and 2534 images in the training and the test sets respectively.

## Attack models

[Adversarial Robustness Toolbox](https://adversarial-robustness-toolbox.readthedocs.io/en/latest/modules/attacks/evasion.html) is used for [DeepFool attack](https://adversarial-robustness-toolbox.readthedocs.io/en/latest/modules/attacks/evasion.html#deepfool) and [Carlini & Wagner l2](https://adversarial-robustness-toolbox.readthedocs.io/en/latest/modules/attacks/evasion.html#carlini-and-wagner-l-2-attack)         
[CleverHans](https://github.com/cleverhans-lab/cleverhans) is used for FGSM and PGD.    
[PyTorch library](https://pytorch.org/tutorials/beginner/fgsm_tutorial.html) is used for the implementation of the models.  

## Codes
The following jypyter notbook have the deep learning and attack models implemented in Pytorch.
First, we trained VGG16 and ResNet50 models on the BTSC dataset. Then, we applied four attacks to create non-targeted adversarial examples using the test set, by using five perturbation magnitudes( epsilons = [0, 5/255, 10/255, 20/255, 50/255]. In the third step, we created targeted white-box evasion attacks using FGSM, PGD, DeepFool, and arlini & Wagner l2 attacks. https://github.com/AzadehNk/White-box-evasion-attacks-on-the-BelgiumTS-BTSC-dataset/blob/main/ADML_%20GitHub.ipynb
## Citation
This project is based on an assignment for [Adversarial Machine Learning course (CS 404-504) at Computer Science Department at University of Idaho](https://www.webpages.uidaho.edu/vakanski/CS_504.html)
