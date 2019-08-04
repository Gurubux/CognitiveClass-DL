# CognitiveClass-DL
<a href='https://cognitiveclass.ai/learn/deep-learning/'>Cognitive Class Deep Learning</a><br>
### 1. Deep Learning Fundamentals<br>
### 2. Deep Learning with TensorFlow<br>
### 3. Accelerating Deep Learning with GPU<br>

<hr>
<br>
##DEEP NEURAL NETWORKS
### 1. CNN<br>
	- Automatic and effective Feature extraction<br>
	- Convolutional Neural Network - Or CNN For short - is a deep learning approach that learns directly From samples in a way that is much more effective than traditional Neural networks. <br>
	- CNNs achieve this type of automatic feature selection and classification through multiple specific layers of sophisticated mathematical operations. Through multiple layers, a CNN learns multiple levels of feature sets at different levels of abstraction. And this leads to very effective classification. <br>
	- Machine vision projects, including image recognition Or classification, such As distinguishing animal photos or <br>
	- Digit recognition, <br>
	- Skin cancer classification. <br>
	- Object detection, For example real-time recognition of passengers in images captured by self-driving cars. <br>
	- Coloring black and white images, and creating art images.<br>
<br>
### 2. RNN<br>
	- Modeling sequential data <br>
	- Stock Market Data<br>
	- We simply need to feed the network With the sequential data, it then maintains the context of the data And thus, learns the patterns within the data<br>
	- Sentiment analysis<br>
	- Language modeling - Predict the next word in a sentence.<br>
	- Text translation - Google Translator<br>
	- Speech-to-text<br>
<br>
### 3. Restricted Boltzmann Machines<br>
	- Find the patterns in data in an "unsupervised" manner.<br>
	- Shallow neural nets that learn to reconstruct data by themselves<br>
	- Unsupervised<br>
		- Feature extraction<br>
		- Dimensionality Reduction<br>
		- Pattern recognition, <br>
		- Recommender systems, H<br>
		- Handling missing values, <br>
		- Topic modeling<br>
<br>
### 4. Deep Belief Network<br>
	- Built on top of RBMs<br>
	- Solves back-propagation problem, "Local-minima" and "vanishing gradients"<br>
	- Solve this by the stacking of multiple RBMs<br>
	- Classification<br>
		- Image recognition<br>
		- A very accurate discriminative classifier - As such, we don’t need a big set of labeled data to train a Deep Belief Network; in fact, a small set works fine because feature extraction is unsupervised by a stack of RBMs.<br>
<br>
### 5. Autoencoders<br>
	- Extracting desirable features<br>
	- Like RBMs, Autoencoders Try to recreate a given input, but do so With a slightly different network architecture and learning method.<br>
		- Autoencoders take a set of unlabeled inputs, encodes them into short codes, and then uses those to reconstruct the original image, While extracting the most valuable information From the data.<br>
		- As the encoder part of the network, Autoencoders compress data From the input layer into a short code -- a method that can be used For               "dimensionality reduction" tasks. <br>
		- Also, in stacking multiple Autoencoder layers, the network learns multiple levels of representation at different levels of abstraction. <br>
			For example, to detect a face in an image, the network encodes the primitive features, like the edges of a face. Then, the first layer`s output goes to the second Autoencoder, to encode the less local features, like the nose, and so on. Therefore, it can be used for Feature Extraction and image recognition.