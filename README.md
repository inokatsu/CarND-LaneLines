# **Finding Lane Lines on the Road** 


---
[//]: # (Image References)

[image1]: ./test_images_output/solidWhiteRight.gif "example_result_gif"
[image2]: ./test_images_output/gray.jpg "gray"
[image3]: ./test_images_output/canny_edge.jpg "canny_edge"
[image4]: ./test_images_output/masked_image.jpg "masked_image"
[image5]: ./test_images_output/hough.jpg "hough"
[image6]: ./test_images_output/result.jpg "result"

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

![example_result_gif][image1]

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 

1. Convert the image to grayscale

![gray][image2]


2. Define a kernel size and apply Gaussian smoothing
    
3. Run Canny edge-detection on the blurred image, with low and high gradient thresholds

![canny_edge][image3]

    
4. Mask the region of interest on the canny-edged image. 

![masked_image][image4]


5. Hough transformation

![hough][image5]


6. Overlaid the averaged and extrapolated lines on the input image.

![result][image6]

    
</br>

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when the white or yellow line are covered with snow. 

Another shortcoming could be that if a car with whilte or yellow body cuts in front of my car, the function might not work correctly. 

</br>

### 3. Suggest possible improvements to your pipeline

A possible improvement would be to make the function recognize another car and distinguisch the line on the ground.

