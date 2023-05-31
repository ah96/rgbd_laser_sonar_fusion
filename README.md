# gridmap_laser_rgbd_fusion
#map_img_proccess
@fuction: this is top model,rectified map by 3D obstacle.
@input  : map.yaml map.pgm,"/laser_pose","/keypoint_scan"
@output : rectified_map.pgm

#laser_rgbd_sonar_fusion
@fuction: fuse laser and rgbd,extra keypoint of 3D obstacle.
@input  : "/scan","/xtion_scan"
@output : "/keypoint_scan"

#depthimage_to_laserscan
@fuction: get 3D points from asus_xtion,get 2D scan by 3D points project into x-y plan.
@input  : "depth/image"
@output : "/xtion_scan"

