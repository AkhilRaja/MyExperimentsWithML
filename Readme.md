# ML Quickstart

Just an attempt to solve a couple of questions on ML and my self learning guide.

## Plugins Used

* [sk-learn]
* [plot]
* [numpy]
* [tensorflow]


# 1 Setting 

## 1.1 Objectives

The objective of this assignment is to get you familiarize with the problems of “classification” and “verification” with a popular problem space of “face”. You are provided with
• Datasets (in some standard form)
• Code for feature extraction/classification. (some
from course other from popular library).
What is expected at the end (i) Familiarity with this (a specific) problem space and the associated nu- ances. (ii) some exposure to the visualization of data (iii) conduct experiments and report results (iv) use of graphs/tables to present results (v) decide param- eters yourself (“best” according to you) and defend your choices. (vi) creating a brief report, with examples arguments.

## 1.2 Dataset

You are given 3 different datasets. Each dataset has faces images of humans. You need to perform experiments on these images.
Yale Face Database This is a classical data set. See original data and description at [1]. Worth reading. We have subsampled the following data for this experiment.
• You are given faces images of 15 subjects.
• Each subject has 11 images with different emotions.
• An emotion.txt is also given which contains mapping the emotion of each image.
Indian Movie Face Database This is an Indian data set. See original data and description at [2]. Worth read- ing. We have subsampled the following data for this ex- periment.
• You are given face images of 8 Indian movie actors. • 50 images are provided for each actor.
IIIT Cartoon Face Dataset This is not natural face. But you still recognize. See original data and description at [3]. Worth reading. We have sub-sampled the following data
• Cartoon faces of 8 subjects.
• 100 images are provided for each subject.
You can download and use data from original sources. However, to make life simple, a version is downloaded and shared with you. For each dataset you are given files <a> <b>.pngwhichisthebthfaceimageofath actor.

# 1.3 Image Features

You are expected to use 6 different features/Representations. These are: 
* [ (a) PCA/Eigen face ]
* [ (b) KernelPCA]
* [ (c) LDA/Fisher face]
* [ (d) Kernel Fisher Face]
* [ (e) VGGFace ] 
* [ (f) ResNet]

You are given a sample code for all the above six rep- resentations/features. You can modify or find a better implementation, if you prefer. If there are computational issues, we will consider giving you the features itself di- rectly.
You are free to improve the basic implementa- tions/links provided by us.
# 2 Questions

## 2.1 Basic Questions

1. Understand the “Eigen Faces”. How many eigen vec- tors/faces are required to “satisfactorily” reconstruct a person in these three datasets? (Don’t forget to
You are expected to use 6
tures/representations. These make your argument based on eigen value spectrum. Show appropriate graphs, qualitative examples and make a convincing argument.)
Which person/identity is difficult to represent com- pactly with fewer eigen vectors? Why is that? Ex- plain with your empirical observations and intuitive answers.
Which dataset is difficult to represent compactly with fewer eigen vectors? Why is it so? Explain with your empirical observations and intuitive answers.
2. Use an MLP classifier and find the classification ac- curacy. Which method works well? Do a comparitive study.
You already know the paper “Face Recognition Us- ing Kernel Methods ”. See this as an example for empirical analysis of different features/classification.
3. Use t-SNE based visilization of faces? Does it make sense? Do you see similar people coming together? or something else? Can you do visualization dataset wise and combined?
You might have seen such data visualization plots in the past at different places. Here you will use a popular implementation.
(Worth reading and understanding t-SNE. We will not discuss it in the class and out of scope for this course/exams.)
4. In practice ”face” is used for verification. i.e., in- put is ”identity/classID) and the face image” and response is ”Yes” or ”No”. (i) How do we formulate the problem using KNN (ii) How do we analyze the performance ? suggest the metrics (like accuracy) that is appropriate for this task. Show empirical re- sults with all the representations and variations in K.

## 2.2 Extension/Application


You know the basic pipeline for recognizing face now. Extend this to “one” of the following or similar problems. You are free to use a new dataset that is publicly avail-
able or even create one by crawling from internet.
1. Politicians vs Filmstars in a public data set. (eg. LFW)
2. Age prediction
3. Gender prediction
4. Emotion classification
5. cartoon vs Real
6. your-own-problem


Briefly explain the problem. Why the problem is not trivial.
Why a solution to this may be of some use. Suggest good applications. Suggest good reasons why solving your problem is
Explain your experimental pipeline, splits, evaluation metrics, quantitative results, qualitative results.


## Author

* **Akhil Raja** - *Code* 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments
