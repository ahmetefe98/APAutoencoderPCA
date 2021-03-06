### Advanced practical: Comparison of autoencoder and PCA for dimension reduction on the CIFAR-100 data set ###

+ this folder includes the code for the advanced practical 
+ for more information about the practical, please read the report.pdf (german)
+ all used sources can be found in the report

### Prerequisites ###

To use this code, you need access to:

+ TensorFlow 2.0 or higher
+ Python 3.5-3.7

### Folder structure and content  ###

+ "cluster": This folder has an approach to cluster images with an autoencoder. For clarity, the code is split up into two files. In "functions.py" there are the functions and imports, and the main code is in "main.py". Throughout the save weights, the models don't need to be fit, they only need to load and compile. Moreover, figure 6, "Vergleich echte Klasse und vermutetet Klasse CIFAR-100" from page 8 of the report, is available in a high resolution in this folder. 
+ "data": Here are the informations about the dataset. The file "classnames.py" prints the 100 class names with their numbers attached. This list can also be found in the file "classnames with classnumbers.txt". The file "unpickle.py" works with the data and creates the images of the subfolder data/images/. To use "unpickle.py", you need to download and decompress 'CIFAR-100 python version' from https://www.cs.toronto.edu/~kriz/cifar.html . In images/classes there are five images for each of the 100 class. In images/superclasses there is for each 20 superclasses one image of the classes, which are grouped in this superclass.
+ "nearest_neigbours": In this folder, the nearest neighbors can search. In the subfolder autoencoder, the dimensions of the images were reduced with the autoencoder. For clarity, the code is split up into two files. In "functions.py" there are the functions and imports and the main code is in "main.py". Throughout the save weights, the models don't need to be fit, they only need to load and compile. The current code searches the nearest neighbors for a random image. To search for a specific image, please change the line 36 "n = randrange(50000)" to the specific image's id. In the subfolder, PCA remains the same, but now the code can only be found in one file. In the subfolder, comparison are the files that are necessary to create the table "Comparison nearest neighbors" from the report. "analyse.xlsx" is the excel file of the table.
+ "reconstruction_loss": In this folder, you can find the code to create the table "Comparison reconstruction loss" from the report. "analyse.xlsx" is the excel file of the table.


### Author ###

+ Ahmet Efe, email: im224@stud.uni-heidelberg.de

31.01.2021 Heidelberg, Germany
