# NeuralNetwork
Created a neural network class that allows you to test different parameters to make the best model for the Auto dataset

Running The Code-----------------------------------------------------------------------

You may simply run the "ml-assignment2.py" code file using Google collab.

In the output code, you will see a summary of each Trial, given the "Trial #", hyperparameters used, and its corresponding accuracy and error. Please note that the graph contains a table of the trial number, number of epochs, and the color-coded line it corresponds too. If you which to know which hyperparameters were used for that specific trial number, simply scroll through the output table to see which trial number the line in the graph corresponds to.

Note: You will see a warning saying, "<ipython-input-10-c9d8b4e2f4e7>:150: FutureWarning: The frame.append method is deprecated and will be removed from pandas in a future version. Use pandas.concat instead.
  output = output.append(combo, ignore_index = True)"
This is not an error. It is simply a warning to use a different method of appending to a dataframe in the future. For now, it works with the current version of pandas. Thanks!

HEADS UP:
The code keeps track of epochs and accuracy for all possible cases of the hyperparameters listed in the instructions.
Appologies, but because of this, it will take a very LONG time to compile, as all of this data must be plotted like the instructions mentioned.

IMPORTS---------------------------------------------------------------------------------

Imports should already be in the code that I submitted, but just in case you want
reference for the imports used, they will be listed below for each part.

import numpy as np
import pandas as pd
from sklearn.model_selection import train_test_split
import keras
from keras.utils import to_categorical
from keras.models import Sequential
from keras.layers import Dense
from sklearn.metrics import recall_score
from matplotlib import pyplot as plt
from itertools import product
