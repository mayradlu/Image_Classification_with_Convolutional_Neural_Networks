# Classification with Convolutional Neural Networks
## General Information
In the digital revolution era, image analysis has become a crucial task, driven by advancements in artificial intelligence. This project focuses on applying Convolutional Neural Networks (CNNs) to three different datasets, aiming to achieve a high level of accuracy in classification and recognition tasks.

## Data Description
Fashion-MNIST
* Size: 70,000 images (60,000 for training and 10,000 for testing).
* Description: Grayscale images, 28x28 pixels, representing 10 classes of clothing items (shirt, pants, sweater, dress, coat, shoes, t-shirt, sneakers, bag, boots).
<p align="center">
  <img src="https://github.com/user-attachments/assets/f801ae74-6ee1-4a98-aac2-e505870d0db4" alt="imagen" width="400">
</p>



**Satellite Images of Mexico**
* Size: 1,636 images.
* Description: High-quality satellite photos showing environments such as Water, Forest, City, Crops, Desert, and Mountain.
* [Database](https://drive.google.com/drive/folders/1yGcbQ6B4GoTHrbmBPHRFVF1dMFafQrpN?usp=sharing) 
<p align="center">
  <img src="https://github.com/user-attachments/assets/154c0dd6-7cc9-415d-a874-cdf7d1d93952" alt="imagen" width="400">
</p>



**Custom Images**
* Size: 2,500 images (500 per class).
* Description: Images captured from different angles and lighting conditions, showing a shoe, a cap, a cellphone, a pencil, and a book.
* Database
<p align="center">
  <img src="https://github.com/user-attachments/assets/034ae7ba-14ab-4c45-b3ba-87d16ada8db5" alt="imagen" width="400">
</p>

## Model Architecture 
The model does the following
* **Conv2D (Convolutional) layer**: 32 filters with a kernel size of (3, 3) and ReLU activation function.
* **Conv2D (Convolutional) layer**: 64 filters with a kernel size of (3, 3) and ReLU activation function.
* **MaxPooling2D (Maximum Pooling) layer**: Reduces dimensionality using a pooling size of (2, 2).
* **Dropout layer**: Randomly turns off 25% of neurons to prevent overfitting.
* **Flatten layer**: Transforms the output into a one-dimensional vector.
* **Dense (Fully Connected) layer**: 128 neurons with ReLU activation function.
* **Dropout layer**: Randomly turns off 50% of neurons.
* **Dense (Fully Connected) layer**: Number of neurons equal to num_classes (output classes) with Softmax activation function

## Training Results
* **Fashion-MNIST** The model was trained for 10 epochs, achieving an overall accuracy of 0.93 on the test set.
<p align="center">
  <img src="https://github.com/user-attachments/assets/7860f969-5d0b-4e6a-a01c-cb05305b15bd" alt="imagen" width="400">
</p>


* **Satellite Images** Trained for 10 epochs, with an accuracy of 0.94 on the training set and 0.82 on the validation set.
<p align="center">
  <img src="https://github.com/user-attachments/assets/8c443868-eee2-4a64-9471-6b11786aab20" alt="imagen" width="400">
</p>


* **Custom Images** Only 3 epochs were needed to achieve an accuracy of 0.99
<p align="center">
  <img src="https://github.com/user-attachments/assets/312f953a-c6f9-43ba-9b63-0f3eca899825" alt="imagen" width="400">
</p>
 
