# loam_velodyne with bug fix
original repo from https://github.com/laboshinl/loam_velodyne

Bug fix:

 - In `LaserOdometry.cpp` line 484, changed the `cornerPointsSharpNum` to `laserCloudCornerLastNum`
 - In `LaserOdometry.cpp` line 595, changed the `surfPointsFlatNum` to `laserCloudSurfLastNum`


There is another bug on mapping node, which is required to publish `/aft_mapped_to_init` with minimum 5 HZ (however the paper claimed to be minimum 1 HZ), further modification on mapping node will be released in this repo to fix this bug.