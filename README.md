**potato disease classification**

number of potato images - 1485

Categories in the dataset are:
['Early_Blight', 'Late_Blight', 'Healthy']

Train Model
To train on Optimized Text CNN
python ADAM_optmized_train.py

Lightweight Text CNN
python singleADAM_LW_train.py

Lightweight TextCNN with Dual Optimizer
Switches from Adam to SGD when a triggering condition is satisfied. python SWAT_LW_train.py

Optional arguments:
python train.py --help

Evaluate Model
To evaluate, run below command

python eval.py --eval_train --checkpoint_dir="./runs/trained_model/checkpoints/"

To use your own data, change the eval.py script to load your data.

Test Model
To prediction on new test data, make sure evaluate model is working , Then run below :

python test.py --out_test --checkpoint_dir="./runs/trained_model/checkpoints/" --test_dir="path to test data"

Link to the paper
For more details please go through my paper at link: https://arxiv.org/pdf/2004.07922.pdf

References :
https://github.com/dennybritz/cnn-text-classification-tf
