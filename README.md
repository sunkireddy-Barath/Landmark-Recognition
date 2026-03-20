# Landmark Recognition System

**Author**: Sunkireddy Barath  
**Year**: 2026  

## Overview
The Landmark Recognition System is a computer vision project designed to identify and classify famous landmarks from images. The system uses deep learning techniques such as Convolutional Neural Networks (CNNs) and Transfer Learning to analyze visual features and accurately recognize landmarks from Google Street View–like images.

## The Neural Network
* **99% accuracy** on validation (static tests)
* **91% accuracy** on test (dynamic tests)
* **Classification error** = 1%
* **Test error** = 9%

![Confusion matrix](Landmark-Recognition-with-Keras-master/resources/confusionMatrixNorm.png)

These are very good results and that is why I have decided to end the training of the network here after 90 epochs and with the training of around ~40,000 images.

## Repository Organization

* **data**: In the data folder you can find all the images I used to train the Neural Network:
  * Training Images
  * Validation Images
  * Test
  
  In the `test` folder you can watch the videos where I show the Neural Network working.

* **resources**: Resources for this readme, primarily the confusion matrix.

* **Dataset Refinement.ipynb**: All the code used to process and modify the original images is in this notebook.

* **Dynamic Test.ipynb**: All the code used to read a video and test the neural network on it is in this notebook.

* **Neural Network for Desktop.ipynb and Neural Network for Google Colab.ipynb**: In these notebooks you can find all the code used to train the CNN and you can select where you want to execute them; on your local computer or in Google Colab. In both, you can execute the static tests (validation).

* **neural_network.h5**: A `.h5` file with the final CNN trained. You can load it with Keras as shown in the Jupyter Notebooks in this way:
```python
from keras.models import load_model
model = load_model(path + 'neural_network.h5')
```

## Contributing
Please open an issue to discuss what you would like to change. 

Thanks for reading! (^.^)
