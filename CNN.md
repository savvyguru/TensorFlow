###Translation Invariance
* max pooling downsamples the image and reduces resolution
* too many max pooling layers results in images that are not positionally correct but with the relevant features are wrongly classified
* instead of having too many layers, data augmentation can be done to maintain translation invariance while not having false positives

###feature extraction
* first few convolution layers picks up edges,textures
* subsequent convolution layers picks up higher order features from this low level features
* standard neural network would pick up all the pixels in the image which is unecessary
* standard neural network is not translation invariant

###relu function
* to introduce non-linearity relationship between all the features
* makes all negative values zero

###filter vs kernel
* kernel is convolution for single channel while filter is for all 3 color channesl
* layered 3X3 kernel size has fewer parameters than a 5x5 kernel, thus model has less parameters to train
* convolutins is a linear transform
* different filters can do operations like edge detection,blur, sharpen edges (think sobel derivative)

###padding
* zero padding done for kernels centered on edge pixels

###strides
* distance we move the kernels by

###transfer learning
* since feature extraction is quite similar for most uses, it is faster to train on pre-trained weights

###fully connected network
* for image classification

###pooling
* downsampling to reduce number of parameters of the model
