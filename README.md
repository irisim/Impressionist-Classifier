# **Impressionist Classifier Project**
The aim of this project is to build a multi-class classifier for 5 impressionist painters, namely: Camille Pisarro, Claude Monet, Henri Matisse, John Singer-Sargent , and Vincent van Gogh.

The Data set is downloaded from:
https://www.kaggle.com/datasets/delayedkarma/impressionist-classifier-data

# ***PROJECT OUTLINE***


1.   Prepare the Data
2.   Build training functions and basic CNN
3.   Train CNN called Arti and show results
4.   Train CNN with dropout called Dropi and show results
5.   Use Ensemble Voting and show results
6.   Train an untrained RESNET from torchvision.models and compare results
7.   Train a pretrained RESNET from torchvision.models and show results
8.   Conclusions
9.   Summery

# **PROJECT SUMMARY**

In this project, I attempted to train neural networks for classifying paintings by five Impressionist painters: Camille Pissarro, Claude Monet, Henri Matisse, John Singer-Sargent, and Vincent van Gogh.

I compared four neural network models:

1.   A simple CNN named 'Arti' (accuracy rate of **65%**)
2.   A simple CNN with dropout and layer normalization called 'Dropi' (accuracy rate of **55%**)
3.   ResNet18 (not pretrained) (accuracy rate of **65%**)
4.   Pretrained ResNet18 (accuracy rate of **86%**)

The primary challenge was rapid **overfitting** during training, prompting me to experiment with complexifying the CNN architectures and incorporating dropout and layer normalization. However, these modifications did not yield improvements beyond the maximum accuracy rate of 65%.

To further explore, I thought of comparing my architecture to a state-of-the-art (SOTA) architecture, ResNet18 from torchvision.models. Initially using an untrained ResNet18, I reached the same maximum accuracy rate of 65% after extensive training sessions.

Then I employed the pretrained version of ResNet18, which performed significantly better, achieving an 86% accuracy rate — a 20% improvement compared to all other models. ***This outcome suggests that prior training on diverse categories can indeed enhance artist classification, demonstrating the possibility of transferring knowledge and intelligence across different tasks.***

The ***key insight*** from this project is that you don't have to be confined to your task's original dataset to enhance your network's starting point of intelligence. You can explore the entire world and experiment with other data categories to see how they can benefit your task.
