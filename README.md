## Import Repos
```bash
vcs import < repos.yml
```

## Build workspace
```bash
colcon build --symlink-install
source ./install/setup.bash
```

## Collecting a new bag file at PURT
For PURT facility testing potentially need to set ROS_DOMAIN_ID=0 to match NavQPlus
```bash
ros2 launch purt_uwb_test test.launch
```
