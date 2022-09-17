# Data


# Tagged data

The labeled data for training the network consists of two categories of chart patterns, the double top patterns, and the head and shoulders patterns. In addition to a group that differs from the latter two, being a group of random market movements, without correlation with any of the tagged patterns, in order to use them as a category that differs from the previous patterns at the time of training the model.
These data are found in the "Tagged Data" folder, where each set of patterns was tagged on a different market, and in its file name definition is the name of the financial market on which they were identified. This was done on the four main financial markets such as EURUSD, GBPUSD, USDJPY and USDCHF. Although there are no variations between the patterns identified from one market to another, what was allowed is to take in total a greater number of patterns of a specific category and in the end to obtain a greater number of data with which to train the neural network.

-------------

# Raw data

To label the sets of graphical patterns, to be used for the generation of a neural network model to identify them, we proceeded to use as main data the most important financial markets such as EURUSD, GBPUSD, USDJPY and USDCHF. These markets have a high volume, which leads them to generate movements that unleash the appearance of patterns, this is how they were chosen. The period obtained to obtain them was 10 years, and their source corresponds to the financial data provider QuantDataManager. To obtain the data, we proceeded to request the data from their platform, indicating the financial market and the period of time. These data were used as a starting point to then proceed to search for the graphical patterns needed to train the neural network. 
Due to the weight of these raw financial market data files they are not uploaded to this repository, but they can be accessed from the same QuantDataManager platform, indicating the above mentioned characteristics of the data used.
