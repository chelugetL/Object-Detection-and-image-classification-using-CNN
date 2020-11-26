# Object-Detection-and-image-classification-using-CNN
Datasets used: 17 category flower dataset and Blood RBC dataset
# CNN Architecture for Image Classification:
a. Baseline architecture.
Baseline model created from scratch was used, it contains two False Negatives and three hidden layers. The shape is made up of 32, 64 and 128. ‘ReLu’ is used in this setting for activation, 2 by 2 for pooling size. ‘Softmax’ and ‘ReLu’ activation function was used as dense function (128 and 512). ‘Categorical cross entropy’ is used as the loss function and Adam as the optimiser which changes the learning rate during the training process.
b. Customized architecture.
VGG19 was the second model used, it’s a pre-trained model. The parameters used are similar to the base model excluding the two dense functions which are made up of 1028 with ReLu activation function. Untrainable parameters were used to freeze the first five layers.
InceptionV3 was used as the third pre-trained model with similar settings as the second model above.
# CNN Architecture for Object Detection:
a. Faster RCNN First selected model was done by Faster R-CNN neural network. Faster R-CNN detects objects in two stages: It first recognizes areas of relevance, and then moves these areas to a convolutional neural network. The features resulting from the first two stages are then passed to Support Vector Machine (SVM). TensorFlow Object Detection API has provided R-CNN by default with pre-trained weights.
b. SSD (Single Shot detector) Second Selected model for configuration is ssd-mobilenet-v2, MobileNet-v2 was used to classify the images. It’s a pretrained network with 53 layers. SSD goes straight from image pixels to bounding box.
