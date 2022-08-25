# image_processing
Target:
We have two images, one is Channel0.tif where we can get the feature(ROI) coordiates and ROI size from it, and then using these ROI infomation to extra feature(ROI) signal from Channel1.tif which range from 0 to 65535. 

Given info:
1. You may assume all features with the same size and same distance between each other.
2. Given the threshold (35000), we can use this threshold to filter interested pixels.
3. Two images have no shift, and have the same image size.
4. Please use Python and OpenCV (kindly remind: if you can not process 16bit images directly, for Channel0.tif you can compress it to 8bit first, then get useful ROI information and use this information to extract the ROI signal after that.)
5. Images may contain noise, please filter all these noise.
![image_processing](https://github.com/VibrantIT2021/image_processing/blob/main/noise.jpg)

output:
1. Check chip direction.
2. Calculate chip rotation 
3. Get feature size, Search mark size

![image_processing](https://github.com/VibrantIT2021/image_processing/blob/main/search_marks.jpg)

5. Index features, Consider time efficiency
6. Extract each feature signal along with feature location index (e.g. (0,0), (1,0))
And the result table example:

| Feature index  | Feature signal  | X_axis |  Y_axis |
| -------------| ------------- | ------------- | -------------|
| 1  | 36666  | 100  |200|
| 2  | 36896  | 120  |210|

6. Final processed Channel1.tif should be like this (cropped):
![image_processing](https://github.com/VibrantIT2021/image_processing/blob/main/results.jpg)
