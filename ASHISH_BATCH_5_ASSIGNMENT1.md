# Ashish Kejriwal Batch 5
## Article on Feature Engineering
As mentioned in the session, 2012 was the death of Computer Vision Engineers. The main reason is that previously we used to hand craft the features and on top of them used classification methods like SVM, Decision trees etc. to get meaningful results like for object detection. But using Neural Networks/Deep Learning we don't have to do "Feature Engineering" any more. The network learns the most important features for that task from the input on its own. We don't to hand engineer features anymore. We have to just provide sufficient training dataset to generalize well, and the network learns the best filter in each layer to produce the features.

## Article on Convolution
Convolution has been a useful concept in signal processing especially in image processing. Convolution in spatial domain is equivalent to multiplication in time domain, filter design to get desired output. Low pass filtering requires Gaussian Kernel (Averaging), High pass filtering for edge detection Sobel filter etc. are some examples used in traditional image processing techniques. Similarly Convolution was introduced in Deep Neural Networks for recognizing hand written digits from images. Using CNN the number of parameters decreased significantly and we could use GPU's parallel processing. To genearate one feature map the same filter is processed over the whole image, this reduces no. of parameters and similar processing for different pixels is ideal for single instruction multiple data type of processor i.e. GPU's. Nowadays CNN is not just limited to Computer Vision tasks but also applied for Speech Recognition (1D Conv) and NLP tasks as well.

## Article on Activation Function
Activation Functions adds non-linearity to Neural Network Architecture. By adding non-linearity, the network can learn more complex functions and thus it increasing its learning capacity. If we use linear function at end of every layer, its essentially reduces to using only one layer which makes using deep network pointless. There are various activation functions used in neural networks like
$$ sigmoid(x) = 1 / (1+exp(-x))$$
$$ tanh(x) = (exp(x) - exp(-x)) / (exp(x) + exp(-x))$$
$$ relu(x) = max(0,x)$$

![Sigmoid vs ReLU](https://cdn-images-1.medium.com/max/1600/1*XxxiA0jJvPrHEJHD4z893g.png)





















