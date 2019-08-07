<h1 align=center><font size = 5>Deep Belief Network </font></h1>

One problem with traditional multilayer perceptrons/artificial neural networks is that backpropagation can often lead to “local minima”. This is when your “error surface” contains multiple grooves and you fall into a groove that is not lowest possible groove as you perform gradient descent.

__Deep belief networks__ solve this problem by using an extra step called __pre-training__. Pre-training is done before backpropagation and can lead to an error rate not far from optimal. This puts us in the “neighborhood” of the final solution. Then we use backpropagation to slowly reduce the error rate from there.

DBNs can be divided in two major parts. The first one are multiple layers of Restricted Boltzmann Machines (RBMs) to pre-train our network. The second one is a feed-forward backpropagation network, that will further refine the results from the RBM stack.

<img src="https://raw.githubusercontent.com/Gurubux/CognitiveClass-DL/master/2_Deep_Learning_with_TensorFlow/DL_CC_2_5_Autoencoders/DBNs.png" alt="DBN Model"/>
