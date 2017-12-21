# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)
<img src="examples/laneLines_thirdPass.jpg" alt="laneLines_thirdPass" title="laneLines_thirdPass" width="960" height="540" />

[image1]: ./examples/grayscale.jpg "Grayscale"
<img src="examples/grayscale.jpg" alt="grayscale" title="grayscale" width="300" height="169" />
---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 

    1. Convert the image to grayscale
    
    2. Define a kernel size and apply Gaussian smoothing
    
    3. Run Canny edge-detection on the blurred image, with low and high gradient thresholds
    
    4. Mask the region of interest on the canny-edged image.
    
    5. 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
