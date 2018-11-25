Laneline Detection Pipeline :

Original_Image --> GrayScale --> GaussianBlur --> EdgeDetection(Canny) --> RemovingNoise(Region of Interest)-->Hough_Transform-->DrawLines-->Merge_Original_with_transformed

Following steps are involved in my Laneline Detection Pipeline:
 1. Convert original image to grayscale
 2. Apply gaussian blur filter
 3. Use canny edge detection method for find all edges in the image
 4. Find region of interest by extracting useful section of the image
 5. Use hough transform to get all the lines
 6. draw_lines() method is used to draw/exprapolates lines over detected lanes
 
 
 
 