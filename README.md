# Horse_or_Human_Classifier

The following python code will use the OS library to use Operating System libraries, giving us access to the file system,
and the zipfile library allowing you to unzip the data.

The contents of the .zip are extracted to the base directory /tmp/horse-or-human, which in turn each contain horses and 
humans subdirectories

One thing to pay attention to in this sample: We do not explicitly label the images as horses or humans. 

Here, instead of explicitly labelling the images, we have used something called an ImageGenerator, and  is coded to read images from subdirectories, and automatically
 label them from the name of that subdirectory.
 
 
 Here, we have added convolutional layers, and flatten the final result to feed into the densely connected layers.

Finally we add the densely connected layers.

Note that because we are facing a two-class classification problem, i.e. a binary classification problem, we will end our 
network with a sigmoid activation, so that the output of our network will be a single scalar between 0 and 1, encoding the
probability that the current image is class 1(as opposed to class 0).
