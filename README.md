# rbkairos_sim

Packages for the simulation of the RB-Kairos.

<p align="center">
  <img src="doc/rbkairos.png" height="275" />
</p>

## Packages

### rbkairos_gazebo

This package contains the configuration files and worlds to launch the Gazebo environment along with the simulated robot.

### rbkairos_sim_bringup

Launch files that launch the complete simulation of the robot/s.

## Docker Usage

In order to run this simulation you will need nvidia graphical acceleration

### Installation of required files

- [docker](https://docs.docker.com/engine/install/ubuntu/)
- [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker)
- nvidia-drivers

### Usage

```bash
git clone https://github.com/RobotnikIstobalAI2/rbkairos_sim_upstream.git
cd rbkairos_sim_upstream
git checkout noetic-devel
export ROS_BU_PKG="rbkairos_sim_bringup"
export ROS_BU_LAUNCH="rbkairos_complete.launch"
cd docker
docker compose up
```

