# Histogram Equalization and Matching ⭐

An image histogram is a type of histogram that acts as a graphical representation of the tonal distribution in a digital image. It plots the number of pixels for each tonal value. By looking at the histogram for a specific image a viewer will be able to judge the entire tonal distribution at a glance.

Image histograms are present on many modern digital cameras. Photographers can use them as an aid to show the distribution of tones captured, and whether image detail has been lost to blown-out highlights or blacked-out shadows. This is less useful when using a raw image format, as the dynamic range of the displayed image may only be an approximation to that in the raw file.

### What are Histograms? 🔥

A histogram is an approximate representation of the distribution of some numerical data. It is the most commonly used graph to show frequency distributions. It looks very much like a bar chart. 

In terms of image: 
Histogram is a graphical representation of the intensity distribution of an image. In simple terms, it represents the number of pixels for each intensity value considered.

### Applications of Histograms

Histograms are preferred in applications, when their is a need for any of the following: 

-  The data are numerical and the distribution of data is needed to be observed, especially when determining whether the output of a process is distributed approximately normally or not

- Seeing whether a process change has occurred from one time period to another

- Determining whether the outputs of two or more processes are different

- Statistical properties need to be modeled

Some specific use cases of histograms are

- In hydrology the histogram and estimated density function of rainfall are used to gain insight in their behaviour and frequency of occurrence. 

- In many Digital Image processing programs there is a histogram tool, which show you the distribution of the contrast / brightness of the pixels. 

## Histogram Equalizing 🔥

Histogram equalization is a method for contrast adjustment using the image's histogram.
Basically, it is a computer image processing technique used to improve contrast in images. It accomplishes this by effectively spreading out the most frequent intensity values. When the useable data is represented by near contrast values, this approach generally boosts the global contrast of pictures. This enables locations with poor local contrast to gain a higher contrast.


## Histogram Matching 🔥

Histogram matching is the transformation of an image so that its histogram matches a specified histogram. 
In order to match the histogram of images A and B, we need to first equalize the histogram of both images. Then, we need to map each pixel of A to B using the equalized histograms. Then we modify each pixel of A based on that of B.

Histogram matching may be used to balance detector responses. It can be used to equalise two pictures that were taken in the same place with the same local lighting (such as shadows), but with different sensors, atmospheric conditions, or global illumination.


## Observations :notebook:

### Histogram Equalization 
Comparing with the inbulit results, my custom implementation seems to be reproducing almost similar results.
The image histogram of the inbuilt function and the custom implementation are almost similar. Apart from the
histogram, the contrast of the image itself has been improved, and the implementation seems to be performing histogram equalization correctly.


## Histogram Matching 
Comparing with the inbuilt results, both the image and the histogram appear to be almost similar. The purpose of histogram matching also seems to have been achieved as far as it can be. Since the source and the destination images are completely different one, therefore tha matching is not perfect. However the overall lighting and contrast seems to have been matched to the destination image. 


## Instructions to Run :runner:

* The dataset is being downloaded from the given hashed link. However if at a later point of time, the dataset is not available in the input file, kindly use the dataset present in the repository in place of the downloaded data. 

* To run, open the python notebook file and select the image number using the slider given. Then run the corresponding cells to get the results

## References and Credits 💳

1. Muhammad Ali Qureshi, Azeddine Beghdadi, and Mohamed Deriche. Towards the design of a consistent image contrast enhancement evaluation measure. Signal Processing: Image Communication, 58:212–227, 2017.
2. https://en.wikipedia.org/wiki/Histogram_equalization
3. https://en.wikipedia.org/wiki/Cumulative_distribution_function
4. https://en.wikipedia.org/wiki/Histogram_matching
5. http://paulbourke.net/miscellaneous/equalisation/