```
[0.026954950989454846, 0.9928]
```

**Convolution:**
Convolution is the process of visiting each pixel of the image to retrieve the information from the image. The information retrieved will be dependent on the type of filter the image will be convolved on.

**Filters/Kernels:**
Filter/Kernels are the matrices that helps in extracting different types of features from the image. For example a kernel can extract only horizontal edges of an image.

**Epochs**:

Process of visiting all the images/data once by the network while training is called epoch. If the network sees the data 5 times we call them 5 epochs.

**1x1 Convolution:**

1x1 convolution can be used for feature extraction by an exact number we require. we can increase or decrease the number of features by 1x1 convolution by merging or separating the features.

**3x3 Convolution:**

3x3 convolution sees the image  as a set of 3x3 matrix at a time and combines the product to form a single pixel out of it.

**Feature Maps:**

Feature map is the output of the image after applying the filter/kernel.

**Activation Function:**

Activation function decides the neuron to be active or not depending on the value/weight it carries form the previous layers.

**Receptive Field:**

Receptive field is the area of the image visible to the output pixel. For example if a 3x3 convolution is done on a large image twice the receptive field of each pixel is 5x5. If done thrice its 7x7. Its how far the pixel has seen the image.