# Siamese-font-similarity
A Siamese network which uses one shot learning to compare two characters belonging to a veriety od 23 alphabet spaces and recognizes the similarity using L2 distance using a custom created 10-layer CNN later passed into a softmax unit.

## About
This project has been primarily made to give me a deeper understanding of One shot classification , data augmentation and using Google Colab for Computer Vision problems. This character similarity checker achives a 83% accuracy using 5 conv layers, 4 max pooling layers , 1 dense layer and 1 softmax layer. The test images have been augmented and noise has been induced. The L2 distance between the datas' softmax matrix is collected and is matched with the character with the most similar L2 matrix. 

## Working
For detailed working, please visit this paper: <a href="http://www.cs.utoronto.ca/~gkoch/files/msc-thesis.pdf"> Siamese Neural Networks for One-Shot Image Recognition , Gregory Koch. </a>

For a vague understanding, we propose two CNN's with same designs and parameters. We pass two images simultaneously into these and then get a softmax ouptput. The loss is then computed in the following ways:

- If the two images are similar, the softmax output matrices should be similar.
- Else, if the two images are not similar, the softmax output matrices should be varying.

Hence , we use Binary crossentropy to calculate the loss along with an Adam Optimizer to reduce the loss.

## Platforms, libraries and frameworks used

- Google Colab
- CUDA
- CUDAnn
- Tensorflow
- Keras
- Scikit
- Scipy
- Numpy
- Matplotlib

## Contributor(s)

<a href="https://github.com/nickinack">Karthik Viswanathan</a>
