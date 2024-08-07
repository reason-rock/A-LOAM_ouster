# A-LOAM_ouster
## Advanced implementation of LOAM - With Ouster LIDAR

A-LOAM_ouster is and modified version of [A-LOAM](https://github.com/HKUST-Aerial-Robotics/A-LOAM), which uses Ouster LIDAR instead of velodyne.<br>
This code has been fixed by a junior developer, which could cause unexpected problems. (It works fine in my environment at this point.)<br>
If you ask for a pull request in case of a problem, we will actively reflect it.


**Modifier:** [reason-rock](https://github.com/reason-rock)



## 1. Prerequisites
### 1.1 **Ubuntu** and **ROS**
Ubuntu 64-bit 20.04
ROS Foxy


### 1.2. **Ceres Solver**
Follow [Ceres Installation](http://ceres-solver.org/installation.html).

### 1.3. **PCL**
Follow [PCL Installation](http://www.pointclouds.org/downloads/linux.html).


## 2. Build A-LOAM_ouster
Clone the repository and catkin_make:

```
    cd ~/catkin_ws/src
    git clone https://github.com/reason-rock/A-LOAM_ouster
    cd ../
    catkin_make
    source ~/catkin_ws/devel/setup.bash
```

## 3. Run with bagfile(or live Sensor Data)
Prepare Data of OS1-32

```
    roslaunch aloam_velodyne aloam_ouster.launch
    rosbag play YOUR_DATASET_FOLDER/YOUR_BAGFILE
```





## 6.Acknowledgements
Thanks for LOAM(J. Zhang and S. Singh. LOAM: Lidar Odometry and Mapping in Real-time) and [LOAM_NOTED](https://github.com/cuitaixiang/LOAM_NOTED).<br>
Thanks for [A-LOAM](https://github.com/HKUST-Aerial-Robotics/A-LOAM)([Tong Qin](http://www.qintonguav.com), [Shaozu Cao](https://github.com/shaozu))

