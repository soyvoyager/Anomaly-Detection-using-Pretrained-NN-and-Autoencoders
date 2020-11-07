# Anomaly-Detection-using-Pretrained-NN-and-Autoencoders
This is implementation of Anomaly detection problem in case of Image dataset. 
The dataset have two classes as cloud and Non-cloud. Where non-cloud is normal behavior and cloud is anomaly which we want to detect. 
Go through the methodology given below to get known about implementation.


To find anomaly(Cloud images) we will train our model only with non-anomaly(Non Cloud images) data. So that our model can understand non anomaly data more, than anomaly data. We will train it with pre pre-trained CNN model called VGG19. VGG19 is a huge pre-trained convolutional neural network created by IMAGENET. We are using VGG19 by method of Transfer Learning. In case of Transfer learning the used model had been already trained with different problem statement. This method is really flexible as it allows feature extraction, preprocessing and can be directly integrated into another new model using a pretrained model.Transfer learning has the Advantage of reducing the training time of a neural network model and further it could result in less generalization error.


When we train our model with non-anomaly data, Reconstruction_loss will be less for our non-anomaly data when compared to anomaly data. We are also going to use Autoencoders here. Autoencoder is an unsupervised artificial neural network that learns how to efficiently compress and encode data then learns how to reconstruct the data back from the reduced encoded representation to a representation that is as close to the original input as possible. Let’s dive into autoencoders to know them well :


Encoder: It is similar to any simple ANN model. In which the model learns how to minimize the input dimensions and compress the input data into an encoded representation.
Bottleneck: It is nothing but a hidden layer which contains the compressed representation of the input data.
Decoder: The decoder model learns how to reconstruct the data from the encoded representation to be as close to the original input as possible.
Reconstruction Loss: This is the method that measures how well the decoder is performing and how close the output is to the original input.


We can use AutoEncoders for denoising as well. Here we are passing anomaly data to model as an input and training it to remove the noise from the data.
