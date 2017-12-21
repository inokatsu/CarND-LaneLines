# **Finding Lane Lines on the Road** 


---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)
<img src="examples/laneLines_thirdPass.jpg" alt="laneLines_thirdPass" title="laneLines_thirdPass" width="960" height="540" />

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 

    1. Convert the image to grayscale
    <img src="test_images_output/gray.jpg" alt="gray" title="gray" width="1280" height="960" />
    
    2. Define a kernel size and apply Gaussian smoothing
    
    3. Run Canny edge-detection on the blurred image, with low and high gradient thresholds
    <img src="test_images_output/canny_edge.jpg" alt="canny_edge" title="canny_edge" width="1280" height="960" />
    
    4. Mask the region of interest on the canny-edged image. 
    <img src="test_images_output/masked_image.jpg" alt="masked_image" title="masked_image" width="1280" height="960" />
    
    5. Hough transformation
    <img src="test_images_output/hough.jpg" alt="hough" title="hough" width="1280" height="960" />

    6. Overlaid the averaged and extrapolated lines on the input image.
    <img src="test_images_output/result.jpg" alt="result" title="result" width="1280" height="960" />
    
    

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when the white or yellow line are covered with snow. 

Another shortcoming could be that if a car with whilte or yellow body cuts in front of my car, the function might not work correctly. 


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to make the function recognize another car and distinguisch the line on the ground.

