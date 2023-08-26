# Image_recogination
In this project, you’ll train a computer to recognise the numbers between zero and nine. You’ll also learn to measure how well your machine vision model performs the job you have trained it to do.

### What will you learn
- How nodes and layers work in a machine learning model
- How to build a complete model
- How to measure the improvement of your model during its training

### Build Model
- The image classifier you’ll build is a kind of neural network. Neural networks get their name because they behave a little like our brains, which are made of neurons. However, a neural network that you build in a computer uses nodes instead of neurons. The nodes are organised into layers, with every node in a layer being connected to every node in the next layer.<br>
- The first layer takes the input, in this case the image of a number, and the last layer provides the output, in this case the likelihood that the input is each of the numbers from zero to nine. Treat the highest likelihood as the model’s prediction, or best guess, as to what the image is.<br>
- Each node learns a rule, and produces a measure of the strength of the match from its inputs to the rule it has learned, which it passes on to every node it is connected to as an input. Each node is connected to every node in the next layer.

### Compile your model
The metric you’ve added is ‘accuracy’ — this is a percentage measure of how many images the model guessed correctly. The optimizer knows this by checking the image against its label after the model has made a guess. When you train the model, you’ll watch this value go up. A score of 1.0 for accuracy is 100 percent, it would mean the model got everything right.

### Train your model
Create a history variable and assign the output of model.fit() to it (remember that training is sometimes called fitting). Pass the training and validation data you prepared, along with the size of the batches you want to break the data into, and the number epochs — complete runs through the data — you want the model to do before it finishes training. A batch size of 100 and 10 epochs seem to work well for this model.

Below the call to model.fit(), add a call to the plot_accuracy_and_loss() function provided with the notebook, to produce a graph of how your model improved over time. Pass it the history variable you just created.

### More about plot_accuracy_and_loss(history) method
The plot_accuracy_and_loss() function takes a history object as input. This object is returned by the fit() method of a Keras model. The history object contains a dictionary of metrics, including the training and validation accuracy and loss.
The function first extracts the accuracy and loss values from the history object. It then plots the accuracy and loss values on two separate subplots. The first subplot shows the training accuracy and loss, and the second subplot shows the validation accuracy and loss.
The function also sets the labels for the axes and the title for each subplot. Finally, it calls the plt.show() function to display the plot.


