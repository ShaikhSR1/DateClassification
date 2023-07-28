# Date-Classification-App
# An Image-based Android Application for Date Fruit Classification using Convolutional Neural Network
##### A Project Report submitted to the Department of Computer Science and Engineering, Jahangirnagar University in partial fulfillment of the requirements for the degree of B.Sc. in Computer Science and Engineering

#### Release
APK [Link](https://github.com/ShaikhSR1/DateClassification/releases/tag/Initial)


# Declaration

The research work entitled **“An Image-based Android Application for Date Fruit Classification using Convolutional Neural Network”** has been carried out in the **Department of Computer Science and Engineering, Jahangirnagar University** is original and conforms the regulations of this University. I understand the University’s policy on plagiarism and declare that no part of this project has been copied from other sources or been previously submitted elsewhere for the award of any degree or diploma.

# Algorithim

Algorithm-1: System Algorithm
1. Import/collect the data

2. Pre-process data. Define the parameters of image size,batch size for model

3. Dividing the data into training and validation set

4. Creating the `Keras` model.We are using the Sequential model.
    The model is consists of three convolution blocks.
   - Conv2D
   - MaxPooling2D
   - Dense
In each block use ‘relu’ as activation function

6. Compile the model. Use ‘adam’ as optimizer.

7. Run epochs

8. Test the model using date images.

9. Generate ‘TensorFlow Lite’ model from the Keras Sequential Model. 

This ‘TensorFlow Lite’ model will be imported into mobile application for on device machine learning result.

# Application interface

![App Interface](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Application%20Interface%201.png)
![App Interface](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Application%20Interface%202.png)

![CNN](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/CNN.png)

![Model for our projecr](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Model%20for%20our%20project.png)

![Model Performance](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Model%20Summary.png)

| Models | Activation Function | Activation Function | Activation Function |
| ----------- | ----------- |  ----------- |  ----------- |
| Model-1 | ReLU | ReLU | ReLU | 
| Model-2 | ReLU | ReLU | Softmax |  
| Model-3 | TanH | TanH | TanH | 

**Accuracy comparison of the experimented models.**

| Models | Epoch 1 | Epoch 13 | Epoch 25 |
| ----------- | ----------- |  ----------- |  ----------- |
| Model-1 | 0.2494 | 0.9638 | 0.9947 | 
| Model-2 | 0.1831 | 0.5365 | 0.5463 |  
| Model-3 | 0.1138 | 0.1439 | 0.1341 | 


### Performance of model 1
![Performance 1](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Performance%20Graph%201.png)


### Performance of model 2
![Performance 2](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Performance%20Graph%202.png)


### Performance of model 3
![Performance 3](https://github.com/ShaikhSR1/DateClassification/blob/Editing/ProjectReport/Performance%20Graph%203.png)

# Motivation

Date Fruit is also very popular in Bangladesh. In Bangladesh, date fruit categorization is significant because it helps to ensure that customers have access to high-quality date fruits that fulfil particular standards for safety, quality, and freshness. These standards have been established by the government. The categorization of date fruits entails evaluating the fruits according to their size, colour, texture, and other features. This helps to assess the fruits' market worth and whether or not they are suitable for a variety of uses.

Date fruits are traditionally categorised in Bangladesh according to their size and quality, with larger and higher-quality fruits bringing in higher costs at the market. This helps to ensure that farmers are compensated for producing fruits of a high quality, while also allowing customers to  choose from a variety of products that cater to their own interests and requirements. 

In addition, as it offers a standardised method for recognising and labelling the many kinds of fruits, date fruit categorization can contribute to the reduction of instances of fraud and misrepresentation that take place in the commercial sector. This can serve to establish customer trust and confidence in the market, and it can ensure that everyone participating in the supply chain, from farmers to distributors to retailers, is held to the same standards of quality and transparency. This can help to build consumer trust and confidence in the market.

# Why CNN

CNN-based approaches are naturally considered the most suited and effective answer to the problem of date classification, notwithstanding the good results obtained by conventional methods. For similar categorization problems, computer vision systems have been a rapidly expanding field of study. Convolutional neural networks (CNNs) have widespread acclaim in the field of vision-based systems as a powerful mechanism for image categorization problems. CNNs have also been studied in the context of date categorization for the automation of jobs like as harvesting, sorting, and packing in recent years. What we mean by "convolutional neural networks" (CNNs) is a class of deep learning algorithms that take an input image and transform it by giving different features different weights and biases. CNNs' main advantage over more basic methods is that they can identify (and consequently categorize) unique characteristics with relatively little training data. Convolutional, pooling, and fully connected layers are only some of the common types of layers found in CNNs, and they each serve a distinct function. Many methods, including CNN-based ones, have been proposed for classifying date fruits. The authors of suggest using size, shape, and color to categorize the three distinct date fruit varieties known as Aseel, Karbalain, and Kupro. The overall accuracy for this method was 89.2 percent. Another method suggested here uses a Support Vector Machine (SVM) to reliably categorize five distinct date varieties according to their ripeness, species, and average weights. However, focusing on only one variety of date fruit (Medjool), the authors of [15] compare the efficacy of eight various types of existing techniques.
