# PSNR
In this project, I have applied various types of noises like Salt and Pepper noise, Rayleigh noise, Exponential noise and Speckle noise on various images in rgb, grayscale and black and white format, and then used various filters to remove those noise.
The filters applied include Median filter, Gaussian filter, Weiner filter, Laplacian filter and mean filter to remove the noise. 
Finally, I have calculated PSNR of the respective images before adding noise and after removing noise by using a specific filter. 

The PSNR block computes the peak signal-to-noise ratio, in decibels, between two images. This ratio is used as a quality measurement between the original and a compressed image. The higher the PSNR, the better the quality of the compressed, or reconstructed image.

The mean-square error (MSE) and the peak signal-to-noise ratio (PSNR) are used to compare image compression quality. The MSE represents the cumulative squared error between the compressed and the original image, whereas PSNR represents a measure of the peak error. The lower the value of MSE, the lower the error.

To compute the PSNR, the block first calculates the mean-squared error using the following equation:     


![image](https://user-images.githubusercontent.com/79708114/233837532-b30e2bbc-6d7c-4f27-91d4-2d32fbe81a69.png)

In the previous equation, M and N are the number of rows and columns in the input images. Then the block computes the PSNR using the following equation:     

![image](https://user-images.githubusercontent.com/79708114/233837543-255f370b-8c41-41a3-9c22-0cb8d87c48c4.png)

I have tried to analyse which filter is best for removing which type of noise in images.

Median filter performs better for removing salt-and-pepper noise and Poisson Noise for images in gray scale

Weiner filter performs better for removing Speckle noise and Gaussian noise

Gaussian filter for the Blurred Noise 
