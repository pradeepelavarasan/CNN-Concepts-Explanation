### This project explains some of the key concepts related to Convolutional Neural Networks which plays a key role in Computer Vision
This project was created as part of the External Internship Program V3 with Inkers.ai and The School of AI Bangalore, India
The attachments in this repository are supporting images for the document

Note: All images were created from scratch for the purpose of this assignment and were not downloaded from the internet

------

#### 1) Convolution:

Unlike a fully connected NN where all the nodes of 2 subsequent layers are connected, with convolution layer you will have filter (kernel) convolve the input to give the output.  One of the key advantages of convolution is sharing of parameters. Given that there might be feature detectors that help in identifying a feature (say edge) in multiple places of the image, the need to have lot of parameters is reduced. So we can efficiently train the CNN with fewer parameters and it will also avoid overfitting given the sparse connections. Below is an example: 

![1.JPG](https://raw.githubusercontent.com/pradeepelavarasan/EIP3/6dfbb448539a39e1499153940953f0d699126d8d/1.JPG)

------

#### 2) Filters/Kernels

In CNN, the filters are the feature detectors to detect the features on an input which are the building blocks to help identify and understand the context of the input. In case of image, we will have various degrees of filters in the following sequence: edges & gradients -> textures -> patterns -> parts of objects -> objects -> scene. The filters are also referred to a kernels in lot of academic research papers. Below is an example of a 3\*3 edge detection filter applied on a 6\*6 image input. 

![2.JPG](https://raw.githubusercontent.com/pradeepelavarasan/EIP3/6dfbb448539a39e1499153940953f0d699126d8d/2.JPG)



------

#### 3) Epochs

Epoch in context of the neural network refers to 1 iteration over all the training examples for the learning algorithm (model). The model will try to improve itself by adjusting the parameters after every epoch. Even during the case of mini gradient decent where the model improves after every batch, the epoch still refers to 1 iteration over all the training examples. The number of epochs itself is a hyper parameter which is used for fine tuning the model. Below is a pictorial representation of epochs:

![3.JPG](https://raw.githubusercontent.com/pradeepelavarasan/EIP3/6dfbb448539a39e1499153940953f0d699126d8d/3.JPG)



------

#### 4) 1\*1 convolution

A 1\*1 filter will create a slices of (1\*1\*# of channels) on the input. It will multiple the values in the filter with the corresponding values in all the channels of the input and then apply the RELU activation function.  One of the main use of 1\*1 convolution filter is to reduce the number of channels when the number of channels is very large. Below is an example of how 1\*1 convolution filter is used to reduce the number of channels from 10 to 4. 

 ![4.JPG](https://raw.githubusercontent.com/pradeepelavarasan/EIP3/6dfbb448539a39e1499153940953f0d699126d8d/4.JPG)



------

#### 5) 3x3 convolution

When using a 3\*3 kernel, the dimension of the input will reduce by 2 (assuming stride of 1). The number of channels will depend on the number of kernels used and not depend on the size of the kernel. 3\*3 is the most optimized kernel suggested for CNN based on various academic researches. It also has better center view compared to 2\*2. It is advised to use a stride of 1 when using a 3\*3 kernel. Below is an example of a 3\*3 edge detection kernel used:

![5.JPG](https://raw.githubusercontent.com/pradeepelavarasan/EIP3/6dfbb448539a39e1499153940953f0d699126d8d/5.JPG)



------



------

