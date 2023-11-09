# Deep-Learning

**Prerequisite** 
Just basic knowledge of Python, pandas, and Scikit-learn
It also requires both math and statistical knowledge
We are using TensorFlow, Keras, and neural networks, as well as Python.

1. Neural networks have been around for years, but they have become popular due to the growth in the use of data and the amount of data available publicly.
2. Advancement in Hardware: TPU is a TensorFlow processing unit and GPU 
3. Python and open-source systems; C++ used to be the way, and deep learning programs are now way easier to learn.
4. Deep learning frameworks: Pytorch by Meta and Tensorflow by Google
5. A cloud- and AI-boom-free and accessible environment to work and practice with less cost

---
## What is a Neural Network?

**Single Neuron Neural network**

A classification problem
Using logistic regression, this can be done
The neural network works pair by pair until left by one. Let's say we are having a practical where one of three people goes out to get a value, the other gets results, then this is given to those who check the feedback, and then we know if it is correct or not, and this process can be repeated. and basic adjustments can be made repeatedly, and then the group becomes better at getting answers and insight, and you can then use math and others till you get it perfectly. So basically, like learning to cook, you keep messing it up until you finally get it, when your brain has learned repeatedly to know the size of salt and pepper to put in different portions of food.
When dealing with complex datasets and don't know the features you are looking at, you build a neural network with an input layer, hidden layers, and an output layer.
---
Next, we install Tensorflow, a deep-learning library
The difference between PyTorch, TensorFlow, and Keras and also CNTK by Microsoft, which isn't popular,
Keras is a nice wrap that provides convenience around the three(TensorFlow, CNTK, theano.
a code snippet of it
```python
keras.backend.backend() 'tensorflow'

from keras.models import Sequential
from keras.laye3rs import Flatten, Dense, Activation

model = Sequential()
model.add(Flatten(input_shape = [28, 28]))
model.add(Dense(100, activation= 'relu'))
model.add(Dense(10, activation="softmax"))
```

To use Keras directly from TensorFlow
```python
from tensorflow import keras
model = keras.Sequential([keras.layers.Dense(10, input_shape=(784,), activation='sigmoid')
```
