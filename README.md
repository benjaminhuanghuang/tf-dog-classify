## Reference
- Build Your First Deep Learning Classifier using TensorFlow: Dog Breed Example
    - https://towardsdatascience.com/build-your-first-deep-learning-classifier-using-tensorflow-dog-breed-example-964ed0689430
    - https://github.com/udacity/dog-project
- CS231n Convolutional Neural Networks for Visual Recognition
    -http://cs231n.github.io/neural-networks-1/#quick

## Tensfor flow setup
  Using a common TensorFLow env for all projects
```  
  $mkdir ~/tensorflow
  $ virtualenv --system-site-packages ~/tensorflow              # for Python 2.7
  $ virtualenv --system-site-packages -p python3 ~/tensorflow   # for Python 3.n

  $ source ~/tensorflow/bin/activate
  (tensorflow)$ easy_install -U pip
  (tensorflow)$ pip install --upgrade tensorflow      # for Python 2.7
  (tensorflow)$ pip3 install --upgrade tensorflow     # for Python 3.n
```

## Setup python
```
$ virtualenv --system-site-packages -p python3 venv3

$ . venv3/bin/activate

(venv3)$ pip3 install -r requirements.txt

...
(venv3)$ deactivate
```

## Tensor board
```
  tensorboard --logdir=. --port=8000
```

## CNN
Convolutional Neural Networks consist of multiple layers designed to require **little pre-processing** compared to other image classification algorithms.

They learn by using **filters** and applying them to the images. The algorithm takes a **small square** (or ‘window’) and starts applying it over the image. 
Each filter allows the CNN to identify **certain patterns** in the image. The CNN looks for parts of the image where a filter matches the contents of the image.
The first few layers of the network may detect simple features like lines, circles, edges. In each layer, the network is able to combine these findings and continually learn more complex concepts as we go deeper and deeper into the layers of the Neural Network.
The overall architecture of a CNN consists of an input layer, hidden layer(s), and an output layer. They are several types of layers, for e.g. Convolutional, Activation, Pooling, Dropout, Dense, and SoftMax layer.

- Convolutional Layer : The Conv layer consists of a set of filters. Every filter can be considered as a small square (with a fixed width and height) which extends through the full depth of the input volume.


 - Pooling layers: are used to apply non-linear downsampling on activation maps. In other words, Pooling Layers are aggressive at discarding information but can be useful if used appropriately. A Pooling layer would often follow one or two Conv Layers in CNN architecture.