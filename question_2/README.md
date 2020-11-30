# Named Entity Recognition Task
This repository contains the source code for the task of Named Entity Recognition. The task is to replace the LSTM based word-level encoder on a reference neural network architecture with Convolutional Neural Network (CNN) layers.
The tutorial can be found in [**End-to-end-Sequence-Labeling-via-Bi-directional-LSTM-CNNs-CRF-Tutorial**](https://github.com/jayavardhanr/End-to-end-Sequence-Labeling-via-Bi-directional-LSTM-CNNs-CRF-Tutorial/blob/master/Named_Entity_Recognition-LSTM-CNN-CRF-Tutorial.ipynb)
and it is based on the ACL'16 paper
[**End-to-end Sequence Labeling via Bi-directional LSTM-CNNs-CRF**](http://www.aclweb.org/anthology/P16-1101)

## Installation
The best way to install pytorch is via the [**pytorch webpage**](http://pytorch.org/)

## Setup

#### Creating new Conda environment
`conda create -n pytorch python=3.5`

#### Activate the conda environment
`source activate pytorch`

#### Setting up notebooks with specific python version (python 3.5)
```
conda install notebook ipykernel
ipython kernel install --user
```

#### PyTorch Installation command:
`conda install pytorch torchvision -c pytorch`

#### NumPy installation
`conda install -c anaconda numpy`

#### Download GloVe vectors and extract glove.6B.100d.txt into "./data/" folder
`wget http://nlp.stanford.edu/data/glove.6B.zip`

#### Data Files
You can download the data files from within this repo [**over here**](https://github.com/TheAnig/NER-LSTM-CNN-Pytorch/tree/master/data)

## Content Information
* `data`: Contains all the dataset used in this project

* `images`: Contains diagrams of the neural network architecture

* `models`: Contains the original pre-trained model provided by the tutorial

* `results`: Contains accuracy and loss data from trained models

* Scripts: Below are the scripts of the templates for different variations of models with CNN layers as the word-level encoder. To run each of the scripts:
`python <script_name>.py`

  * `NER-CNN-CNN-CRF`: Contains the python script template for the model with a single layer of CNN word-level encoder

  * `NER-CNN-CNN-Avg1DCRF`: Contains the python script template for the model with a single layer of CNN and an average pooling layer word-level encoder

  * `NER-CNN-CNN-Maxpool1D-CRF`: Contains the python script template for the model with a single layer of CNN and a max pooling layer word-level encoder

  * `NER-CNN-CNN2-CRF`: Contains the python script template for the model with two layers of CNN word-level encoder

  * `NER-CNN-CNN3-CRF`: Contains the python script template for the model with three layers of CNN word-level encoder
