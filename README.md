# Image Landmark and Semantic Point Cloud Matching based Localization

---------------------------------------------------------------------

### Package Install
```
git clone https://github.com/soyeongkim/image_landmark_spc_matching_localization.git
cd image_landmark_spc_matching_localization
catkin_make
source devel/setup.bash
```
---------------------------------------------------------------------
#### Run the demo
##### 1. GPS based Localization
```
roslaunch landmark_matching_localization gps_localization.launch 
```
##### 2. Point Cloud Map Matching Localization
```
roslaunch landmark_matching_localization map_matching_localization.launch 
```
##### 3. Image Landmark and Semantic Point Cloud Map Matching Localization
For using image landmark and semantic point cloud map matching localization, you have to run 3 launch files.
(localization, image segmentation AI, image detection AI)

1. Image Landmark and Semantic Point Cloud Map Matching Localization
```
source devel/setup.bash
roslaunch landmark_matching_localization landmark_matching_localizaion.launch 
```
2. Image Segmentation AI
```
source devel/setup.bash
```
3. Image Detection AI
```
source devel/setup.bash
roslaunch darknet_ros darknet_ros.launch
```

##### Download Semantic Point Cloud Example

You can download semantic point cloud map example file at https://konkukackr-my.sharepoint.com/:u:/g/personal/ksy4200_konkuk_ac_kr/EbZDFZBC7B1OnEJCjov5b9kBhQYyz-_SEbcxMEQ7Tt9JwQ?e=HO9JwO . 
Put this file at src/landmark_matching_localization/map.
