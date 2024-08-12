**potato disease classification**

**data set used**

number of potato images - 1485

Categories in the dataset are:   Here we considered three types potato disesase.  ['Early_Blight', 'Late_Blight', 'Healthy']

**Train Model**

To train the model, the following approach was used:

- **Base Model:** DenseNet201
- **Image Size:** 150x150 pixels
- **Epochs:** 30
- **Base Model Layers:** All layers set to non-trainable


**DenseNet: Efficient CNN for Image Classification**

Lightweight TextCNN with Dual Optimizer
Adusted number of epoches, Switches from soyabean images to potato images means changing file path and file size and explored transfer learning effects by running model with all base layer frozen.

**Evaluate Model**

To evaluate, run below command
test_loss, test_acc = model.evaluate(test_generator, verbose=2)


**Link to the paper**

For further details and methodology, please refer to the original research paper: [Soybean Disease Identification Using Original Field Images and Transfer Learning with Convolutional Neural Networks]
(https://arxiv.org/pdf/2004.07922.pdf)

**References:**

RoboCrop-CNN-WebApp GitHub Repository](https://github.com/nzb0054/RoboCrop-CNN-WebApp)
