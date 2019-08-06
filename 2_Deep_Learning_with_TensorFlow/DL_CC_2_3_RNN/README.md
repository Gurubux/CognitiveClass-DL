<h2>Long Short-Term Memory Model</h2>

The Long Short-Term Memory, as it was called, was an abstraction of how computer memory works. It is "bundled" with whatever processing unit is implemented in the Recurrent Network, although outside of its flow, and is responsible for keeping, reading, and outputting information for the model. The way it works is simple: you have a linear unit, which is the information cell itself, surrounded by three logistic gates responsible for maintaining the data. One gate is for inputting data into the information cell, one is for outputting data from the input cell, and the last one is to keep or forget data depending on the needs of the network.

Thanks to that, it not only solves the problem of keeping states, because the network can choose to forget data whenever information is not needed, it also solves the gradient problems, since the Logistic Gates have a very nice derivative.

<h3>Long Short-Term Memory Architecture</h3>

The Long Short-Term Memory is composed of a linear unit surrounded by three logistic gates. The name for these gates vary from place to place, but the most usual names for them are:

<ul>
    <li>the "Input" or "Write" Gate, which handles the writing of data into the information cell</li>
    <li>the "Output" or "Read" Gate, which handles the sending of data back onto the Recurrent Network</li>
    <li>the "Keep" or "Forget" Gate, which handles the maintaining and modification of the data stored in the information cell</li>
</ul>
<br>
<img src="https://raw.githubusercontent.com/Gurubux/CognitiveClass-DL/master/2_Deep_Learning_with_TensorFlow/DL_CC_2_3_RNN/LSTM_Components.png" width="720"/>
<center><i>Diagram of the Long Short-Term Memory Unit</i></center>
<br><br>
The three gates are the centerpiece of the LSTM unit. The gates, when activated by the network, perform their respective functions. For example, the Input Gate will write whatever data it is passed into the information cell, the Output Gate will return whatever data is in the information cell, and the Keep Gate will maintain the data in the information cell. These gates are analog and multiplicative, and as such, can modify the data based on the signal they are sent.
