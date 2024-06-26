# Build-convolutions-and-perform-pooling
You'll want your DNN to be able to identify the clothing item in pictures with other objects, or where it isn't positioned front and center. To do this, you'll need to use convolutions.
2. What are convolutions?
A convolution is a filter that passes over an image, processes it, and extracts the important features.

Let's say you have an image of a person wearing a sneaker. How would you detect that a sneaker is present in the image? In order for your program to "see" the image as a sneaker, you'll have to extract the important features, and blur the inessential features. This is called feature mapping.

The feature mapping process is theoretically simple. You'll scan every pixel in the image and then look at its neighboring pixels. You multiply the values of those pixels by the equivalent weights in a filter.

For example:

Convolution on image

In this case, a 3x3 convolution matrix, or image kernel, is specified.

The current pixel value is 192. You can calculate the value of the new pixel by looking at the neighbor values, multiplying them by the values specified in the filter, and making the new pixel value the final amount.

Now it's time to explore how convolutions work by creating a basic convolution on a 2D grayscale image.

You'll demonstrate that with the ascent image from SciPy. It's a nice built-in picture with lots of angles and lines.
