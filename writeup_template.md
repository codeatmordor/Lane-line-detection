# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./test_images_output/result_1.jpg "Result1"
[image2]: ./test_images_output/result_2.jpg "Result2"
[image3]: ./test_images_output/result_3.jpg "Result3"
[image4]: ./test_images_output/result_4.jpg "Result4"
[image5]: ./test_images_output/result_5.jpg "Result5"
[image6]: ./test_images_output/result_6.jpg "Result6"


---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

Original_Image --> GrayScale --> GaussianBlur --> EdgeDetection(Canny) --> RemovingNoise(Region of Interest)-->Hough_Transform-->DrawLines-->Merge_Original_with_transformed

Following steps are involved in my Laneline Detection Pipeline:
 1. Convert original image to grayscale
 2. Apply gaussian blur filter
 3. Use canny edge detection method for find all edges in the image
 4. Find region of interest by extracting useful section of the image
 5. Use hough transform to get all the lines
 6. draw_lines() method is used to draw/exprapolates lines over detected lanes


### Output Images
![alt text][image1]
![alt text][image2]
![alt text][image3]
![alt text][image4]
![alt text][image5]
![alt text][image6]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
