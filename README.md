## Face Recognition System

![image](https://github.com/user-attachments/assets/a72905e6-2abf-40ad-9e02-875f58e79b0c)


### Description
This project was developed as part of the Post Graduation Program in AI/ML.
The aim is to develop a Face Recognition System for a movie streaming application using CV techniques.


### Features
 - Develop a UNET based model that uses ResNet as the base for encoder. Additional decoder layers are added to UNET
 - Dataset is developed that uses respecive embedding vectors.  
 - Identify similar images based on distance between embedding vectors
 - Dimensionality Reduction technique is applied and a Support Vector Classifier is used to predict the test images


### Dataset
The image dataset is provided as part of the course



### Results

 - The Face Recognition System segments with a Dice Coefficient of around 65% on Test dataset
 - Embedding Vectors are generated using pretrained VGG16 model and PCA is applied
 - The SVM classifier model can recognise provided test images with accuracy of 96%


### Technologies Used
- **Tools:** Python, Google Colab
- **Libraries:** Pandas, Numpy, Scikit learn,Matplotlib, OpenCV, Tensorflow, Keras


### Key Insights

**Face Detection Model using ResNet**

 - Model performance is satisfactory but can be improved by fine tuning on a larger dataset
 - Data augmentation may not be useful as still shots from movie are likely to have a regular orientation
 - More images may be needed with specific characters with pull-on masks/animated faces but not masked in truth masks, so model can stop recognising these as faces

**Face Recognition System using SVM**

 - Applying PCA on embedding vectors allows to minimise computation needs for the SVM classifier
 - SVM Classifier has a good accuracy of 95% on test data
