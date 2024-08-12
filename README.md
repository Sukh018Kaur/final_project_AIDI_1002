**potato disease classification**

**data set used**

number of potato images - 1485

Categories in the dataset are:     ['Early_Blight', 'Late_Blight', 'Healthy']

**Train Model**

To train the model, the following approach was used:

- **Base Model:** DenseNet201
- **Image Size:** 150x150 pixels
- **Epochs:** 30
- **Base Model Layers:** All layers set to non-trainable


Lightweight Text CNN
python singleADAM_LW_train.py

Lightweight TextCNN with Dual Optimizer
Switches from Adam to SGD when a triggering condition is satisfied. python SWAT_LW_train.py

Optional arguments:
python train.py --help

Evaluate Model

To evaluate, run below command
test_loss, test_acc = model.evaluate(test_generator, verbose=2)

python eval.py --eval_train --checkpoint_dir="./runs/trained_model/checkpoints/"

To use your own data, change the eval.py script to load your data.

Test Model
To prediction on new test data, make sure evaluate model is working , Then run below :

Link to the paper
For further details and methodology, please refer to the original research paper: [Soybean Disease Identification Using Original Field Images and Transfer Learning with Convolutional Neural Networks](https://arxiv.org/pdf/2004.07922.pdf)

References :
RoboCrop-CNN-WebApp GitHub Repository](https://github.com/nzb0054/RoboCrop-CNN-WebApp)
