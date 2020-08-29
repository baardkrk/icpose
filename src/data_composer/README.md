# The Composer
The composer creates batches of augmented datasets in real time. It is written for the Panoptic Studio dataset, and will not work on datasets that is not in the given file structure.

The composer looks at the timing data for a given dataset, and extracts the 3D location for the joints of each person for each depth image. An average depth image is also extracted. 

Input parameters to the composer is the names of the datasets you want for validation and training. It will then mix the training data so each batch will have a wide variety of data to avoid overfitting. 

The composer should be run in a separate thread while training the network, so new batches are ready to be consumed once the network needs them.
