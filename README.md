# Anomaly-Detection-using-Pretrained-NN-and-Autoencoders
This is implementation of Anomaly detection problem in case of Image dataset. 
The dataset have two classes as cloud and Non-cloud. Where non-cloud is normal behavior and cloud is anomaly which we want to detect. 
Go through the methodology given below to get known about implementation.

To find anomaly(Cloud images) we will train our model only with non-anomaly(Non Cloud images) data. So that our model can understand non anomaly data more, than anomaly data. We will train it with pre pre-trained CNN model called VGG19. VGG19 is a huge pre-trained convolutional neural network created by IMAGENET. We are using VGG19 by method of Transfer Learning. In case of Transfer learning the used model had been already trained with different problem statement. This method is really flexible as it allows feature extraction, preprocessing and can be directly integrated into another new model using a pretrained model.Transfer learning has the Advantage of reducing the training time of a neural network model and further it could result in less generalization error.
