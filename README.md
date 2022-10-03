# Graphic patterns GAF_CNN
Repository containing software for the detection of double top and head and shoulders patterns. In addition to the code used to generate the trained model capable of recognizing them, for which the Gramian Angular Field method was used to convert the time series of the market to images, then use these images to train a CNN model. We also add the code used to form the labeled data set, so that we have the labeled patterns to be used to train the network. Finally, the raw data of the main markets used over a 10-year period and the patterns that were labeled are included.

# Code testing:

To modify the code that generates the uploaded model you can use a google colab account. Inside your account on the platform open the "Code_for_labeling_and_training.ipynb" file. Also download the tagged data from the "Tagged data" folder and upload it to your drive folder so that the platform has access to the files. Then run the cells referring to the necessary libraries and functions used to transform the data with GAF and CNN cells.

To use the tool that identifies market patterns you can test it from the colab account. Downloading the trained model "CNN_model_pattern.h5" and the colab file that executes it. In the code you can modify the path from where to get the market data and extend the output of the pattern identification to attach it to a system.

# Tool for pattern identification:

Attached to the trained model files and the module for labeling the data is the document that shows the integration of the above steps into a useful tool for identifying graphical patterns. This tool is divided into two modules, both of which are based on the GAF-CNN method. On the one hand, the first module consists of evaluating the number of chart patterns found in a particular market. While in another module a connection was developed with an API that minute by minute queries the latest Japanese candlesticks, from this data is sought to identify in this last stretch of the market the possibility of the presence of a chart pattern. For this, the data is processed, transformed through the GAF method and using the previously trained model to obtain the level of certainty.
