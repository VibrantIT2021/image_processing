# image_processing
Target:
We have two images, one is Channel0.tif where we can get the feature(ROI) coordiates and ROI size from it, and then using these ROI infomation to extra feature(ROI) signal from Channel1.tif which range from 0 to 65535. And the result table example:
| Feature signal  | X_axis |  Y_axis |
| ------------- | ------------- | -------------|
| 36666  | 100  |200|
| 36896  | 120  |210|

Given info:
1. Given the threshold (35000), we can use this threshold to filter interested pixels.
2. Two images have no shift, and have the same image size.
3. Please use Python and OpenCV (kindly remind: if you can not process 16bit images directly, for Channel0.tif you can compress it to 8bit first, then get useful ROI information and use these information to extract the ROI signal after that.)



output:
1. Check chip direction.
2. Calculate chip rotation 
3. Get feature size, Search mark size
4. Index features, Consider time efficiency
5. Extract each feature signal along with feature location index (e.g. (0,0), (1,0))
 

