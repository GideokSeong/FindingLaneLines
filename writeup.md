# Finding Lane Lines on the road
​
---
**Finding Lane Lines on the road**
​
---
*The usage of fuctions in this project*
    1. Grayscaling
    2. Region Masking
    3. Canny Edge Detection
    4. Hough Transform
    5. Weighted image
    
*The goal of this project*
    1. Implemented a **pipeline** which uses all of the functions mentioned above, 
    so can capture the specific line on the road. 
    2. Using pipeline implemented, can apply for the **video** as well.
​
---
​
### Reflection 
    
   ##### There are 5 major parts in my project.
   1. **GrayScaling** - converts original image to gray-scaled image.
   ![alt text](/test_images_output/0.jpg "GrayScaling")
   2. **Canny Edge Detection** - to detect edges which is a binary image with white pixels.
   ![alt text](/test_images_output/1.jpg "Canny")
   3. **Region Masking** - used for tracing a specific line of the road 
   and utilized vertices which is are 4 integer points here and 
   ignore_mask_color which ignores pixels if those do not meet the criteria.
   ![alt text](/test_images_output/2.jpg "Region")
   4. **Hough Transform** - used for drawing line when we give a specific criteria into the pixels we want to pick up.
    
    This function is used with draw_lines function to draw the line in specific pixels 
    which are drawn by region_of_interest function.
   ![alt text](/test_images_output/3.jpg "Hough")
   5. **Weighted image** - edges through hough and draw-lines functions can be expressed into normal picture. 
   ![alt text](/test_images_output/4.jpg "Weight")
   
### Potential shortcomings and Improvements
    - The pipeline I implemented is limited to straight line, so it has to be applied to curve line too
    So, for the near future, I will apply it.

​
