## Cat Breeds Classification Project
`This project aims to classify different cat breeds using deep learning techniques. The project includes a pretrained Xception model with added custom head layers for fine-tuning on the cat breeds dataset.`
## Dataset
The dataset consists of images of 15 different cat breeds. These images are stored in a RAR file named **CAT_BREEDS_DATASET.rar** 
## Model Architecture
* The model architecture is based on the Xception convolutional neural network, pretrained on ImageNet. 
* The final layers of the Xception model have been replaced with custom head layers to adapt it to the cat breeds classification task. 
* Data augmentation techniques such as rotation, shifting, shearing, zooming, and horizontal flipping have been applied to enhance the model's generalization ability.
* The custom head layers include: ***GlobalAveragePooling2D***, ***Dropout()***, ***Dense layer with 512 units and ReLU activation***, ***BatchNormalization*** and ***Dense layer with 15 units*** 
* The model is compiled with ***Adam*** optimizer with ***learning rate `0.0001`*** and ***categorical cross-entropy loss function***
## Training
 `The pretrained Xception model is fine-tuned on the cat breeds dataset using transfer learning. The first 25 layers of the Xception model are trainable and the reast of the layers are not`
## Usage
To use the pretrained model for cat breeds classification:

1. **Extract the images from cat_images.rar.**
2. **Load the pretrained model using your preferred deep learning framework (e.g., TensorFlow, Keras or Pytorch).**
3. **Use the model to classify images of cat breeds.**

# Evaluation
On the `Test data` the mdoel was able to get accuracy **85%**
