# Transfer-learning-in-CNN

## Introduction
The goal of this project is to practice image classification, a strength of CNN models. Our task is to distinguish the types of clothing worn by the main characters in the photos, categorizing them into four different classes. The difficulty of this problem varies in different contexts. Similar problems are discussed in 'Dive into Deep Learning,' but they involve handling cleaner images. The data for this assignment comes from street snapshots, making the classification task more challenging due to the variability and complexity of real-world street fashion.

## Description
I used a method called transfer learning. A pre-trained model is a saved network that was previously trained on a large dataset, typically on a large-scale image-classification task. Therefore, I can use the pretrained model to a given task with transfer learning.

In this project, I try two ways to customize a pretrained model:

- Feature Extraction: Use the representations learned by a previous network to extract meaningful features from new samples. You simply add a new classifier, which will be trained from scratch, on top of the pretrained model so that you can repurpose the feature maps learned previously for the dataset.

- Fine-Tuning: Unfreeze a few of the top layers of a frozen model base and jointly train both the newly-added classifier layers and the last layers of the base model. This allows us to "fine-tune" the higher-order feature representations in the base model in order to make them more relevant for the specific task.

## Workflow
- ##### Examine and understand the data
- ##### Build an input pipeline, in this case using Keras ImageDataGenerator
- ##### Compose the model
- ##### Train the model
- ##### Evaluate model
