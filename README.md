# image_processing
Target:
Channel0.tif defines feature locations. Based on feature locations in step1 to extra feature signal in Channel1.tif 

Given info:
1. Given threshold (35000)
2. Two images have no shift
3. Please use Python and OpenCV


Requirements:
1. Check chip direction
2. Calculate chip rotation
3. Get feature size, Search mark size
4. Index features, Consider time efficiency
5. Extract each feature signal along with feature location index (e.g. (0,0), (1,0))
 
Result table example:


| Feature signal  | X_Axis |  Y_Axis |
| ------------- | ------------- | -------------|
| 36666  | 100  |200|
| 36896  | 120  |210|
