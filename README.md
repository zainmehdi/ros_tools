ros_tools
============

Whenever I need a simple ros node for processing/visualization, I added it to this respository.
So there is a lot of ros boiler plate code here


bag_extractor 
- takes stereo images from a bag file and write to disk
- written to convert datasets for ScaViSLAM

bag_scripts
- modifying bag files using python scripts

feature_msgs
feature_visualizer
- subscribes to feature msgs and visualize them.  
- Written for viso2

image_filter
- apply standard opencv filters to an image
- tried to use this to fix noisey imagary

image_overlayer
- designed to overlay disparity image with stereo image

image_repair
- subscribe to a ros image, convert to cv::mat, convert back to ros and republish
- written to fix ros_images with image.width != image.step

pcd_writer
- convert a text file of x,y,z coords to a pcd file

tf_broadcaster
- publishes tfs

topic_synchronizer
- subscribes to 2 topics and reports how much out of sync they are.  
- I used this to try and 2 cameras by resetting one camera when it went too far out of sync

trajectory_recorder
- subscribes to tf and writes to disk
