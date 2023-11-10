# Deep-Learning

[Disclaimer : this is what I learnt from Deep Learning Videos on YT by CodeBasics
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
the flatten layer is normal connection,

<img width="300" alt="image" src="https://github.com/honourjesus20/Deep-Learning/assets/96244548/8619983c-fa3f-4013-bc71-4dd5dfac4590">

while the dense layer is interconnected in the hidden layer to the next node

<img width="392" alt="image" src="https://github.com/honourjesus20/Deep-Learning/assets/96244548/0e76f1ef-499d-4ab0-8fe9-cf2124857200">

A pictorial representation of an input and ouput layer

<img width="268" alt="image" src="https://github.com/honourjesus20/Deep-Learning/assets/96244548/f1809cba-209b-4778-a63c-f1f97918310b">

For Image you have have a pixel has a two dimensional array to represent, the image and supply the two dimensional array as input then flatten it to one array, for a 7 by 7 grid, the flatten array will be 49, then the input will be 49 neurons and be propagated to get a 10-output layer., the following has no hidden layer

<img width="437" alt="image" src="https://github.com/honourjesus20/Deep-Learning/assets/96244548/84d8ba0e-3fe9-4da3-93e1-097cea8aad42">

Will always first try to use a simple neural network where you have just input and output, next we have the hidden layers inserted
