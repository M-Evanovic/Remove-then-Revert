# *Removert*
# Remove dynamic points, and then revert static points

## 1. Prerequisites
```
data  
├ poses.txt / pose.csv  
├ Scans  
│  ├ 000001.pcd  
│  ├ 000002.pcd  
│  ├ 000003.pcd  
│  ├ ...  
```

## 2. Build
```
cd ~/catkin_ws/src
git clone https://github.com/M-Evanovic/Remove-then-Revert.git
cd ..
catkin_make
source ~/catkin_ws/devel/setup.bash
```

## 3. Get start
```
roslaunch removert run_scliosam.launch.launch
```

## 4.Parameters
Edit `config/params_mulran_scliosam.yaml` to set parameters:  
`save_pcd_directory`: replace to your path (please use an absolute path)  
`sequence_scan_dir`: scan directory path  
`sequence_pose_path`: pose file path  

## 5. Reference
[code](https://github.com/gisbi-kim/removert.git)  
[paper](https://irap.kaist.ac.kr/publications/gskim-2020-iros.pdf)
```
Kim G, Kim A. Remove, then revert: Static point cloud map construction using multiresolution range images[C]//2020 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2020: 10758-10765.
```
