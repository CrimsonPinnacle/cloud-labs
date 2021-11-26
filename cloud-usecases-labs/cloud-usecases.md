# Exploring Cloud Use Cases with Microsoft Azure

> Hands-on Lab

|                   |                       |
| :---------------- | :-------------------- |
| Cloud Vendor      | **Microsoft Azure**   |
| Proficiency Level | **Cloud  Enthusiast** |
| Tags              |  ![https://img.shields.io/badge/%20-Cognitive%20Services-blue](https://img.shields.io/badge/%20-Cognitive%20Services-blue) ![https://img.shields.io/badge/%20-Machine%20Learning-blue](https://img.shields.io/badge/%20-Machine%20Learning-blue) ![https://img.shields.io/badge/%20-Vision%20API-blue](https://img.shields.io/badge/%20-Vision%20API-blue) |

## Lab Scenario
In this lab, you will explore some use cases enabled by the cloud technologies. You will look at Machine Learning and Cognitive Services.

## What will you learn in this lab?
After completion of this lab, you will be able to:

- Understand how Machine Learning models can be created in the cloud
- Understand how Vision APIs work

## Prerequisites
To complete this lab, you will need the following:

- Reliable internet connection
- A work, school or personal Microsoft Account used to access Microsoft Azure
- A subscription for Microsoft Azure

## Exercises

### Exercise #1: Exploring Azure Machine Learning Studio
The objective of this lab is to explore the capabilities of the Azure Machine Learning Studio.

1. Go to https://studio.azureml.net/ (Links to an external site.) and click on the [Sign In] link in the upper right corner.
2. Sign into Azure Machine Learning Studio using your credentials.
3. Once you are signed into Azure Machine Learning Studio, click on [Samples] at the top of the working area.
4. Find the Anomaly Detection: Credit Risk sample in the list and click on it. You will see the model graph in the working area.
5. Click on the [Save As] button at the bottom of the screen and fill in the following information:
  *Experiment Name* --> `[initials]othercloudserviceslab01`
6. Click on the button to confirm.
7. Click on the [Run] button at the bottom of the working area.
8. A counter in the upper right corner will show the time the experiment is running. Once complete, it will show *Finished running*.
9. Scroll down the model graph to see *Evaluate Model* box and click on the circle at the bottom of the *Evaluate Model* box.
10. Select [Visualize] from the context menu.
11. You will see a graph with the model score on the screen.

#### Exercise Summary
At this point, you have learned how to create and evaluate a machine learning model in Azure Machine Learning Studio.

### Exercise #2: Exploring Azure Vision API

The objective of this lab is to explore the image classification capabilities of Microsoft Vision Cognitive Service.

1. Go to https://azure.microsoft.com/en-us/services/cognitive-services/computer-vision/ (Links to an external site.) and scroll down to show the images and the buttons for upload.
2. Click on the [Browse] button to upload your image to the service.
3. Select a picture from your local machine and upload it to the service.
   **Note:** Use an image that is less than 1 MB else you will receive an error that the image is too big.
4. In the right-side, you will see information about the image like description, tags, categories and so on.

#### Exercise Summary
At this point, you have learned how Microsoft Azure Visiou API can be used to recognize object in images.

## Help improve this lab

[![Lab Issues](https://img.shields.io/github/issues/crimsonpinnacle/cloud-labs)](https://github.com/CrimsonPinnacle/cloud-labs/issues/new?assignees=toddysm&labels=new+lab&template=bug_template.md&title=) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/CrimsonPinnacle/cloud-labs/pulls)