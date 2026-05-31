# Bird Species Image Classifier

## Overview
In this project we are attempting to fine tune 3 different machine 
learning models so that they can identify different species of birds 
at a high accuracy. This machine learning model could help create 
something like an app on a phone that is able to identify birds in 
the wild. This machine learning model could definitely be used in 
other domains as well, more than just personal use, it could be 
used in biological labs to determine what certain things are, maybe 
better than a human.

## Models
Three pre-trained CNN models were fine-tuned and compared:
- **AlexNet**
- **ResNet**
- **VGGNet**

Each model had 3 visualizations produced for a total of 9 visualizations.

## Results
For AlexNet the epoch that performed the best was number 9, for 
ResNet the epoch that performed the best was number 5, and for 
VGGNet the epoch that performed the best was number 9 as well. 
Overall the model with the best performance all around was AlexNet. 
It had a similar confusion matrix to ResNet but instead of getting 
2 incorrect for 1 species it got 1 incorrect from 2 species, and 
one was from the species with less samples than the others.

## Key Findings
VGGNet performed a lot worse than AlexNet and ResNet, at least when 
it comes to this dataset. Normally VGGNet performs better than 
AlexNet, especially when it comes to harder tasks like ImageNet. 
Maybe it didn't perform as well because there were not enough classes 
or the images were not complex enough.

The models already had great results by the first epoch because in 
this project we were just fine tuning them, bringing their already 
good accuracy even higher making them nearly perfect. I don't think 
adding more epochs to these tests would increase the accuracy much, 
most of the time the highest accuracy was not found on the largest 
epoch and the graphs are almost straight lines barely improving each 
time.

Overall this dataset was well suited for an AlexNet model which had 
very impressive results, getting only 2 predictions wrong.

## Technologies
- Python
- PyTorch
- Google Colab (GPU — T4)
- AlexNet, ResNet, VGGNet (pre-trained)

## Usage
Open the notebook in Google Colab and run all cells. A GPU runtime 
is recommended for reasonable training times.
