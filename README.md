# Extended Kalman Filter Project

In this project, I use extended Kalman filter to estimate the state of a moving object by fusing the noisy lidar and radar measurements.

This repository includes two files that can be used to set up and install [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac systems. For windows you can use either Docker, VMware, or even [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. Please see [this concept in the classroom](https://classroom.udacity.com/nanodegrees/nd013/parts/40f38239-66b6-46ec-ae68-03afd8a601c8/modules/0949fca6-b379-42af-a919-ee50aa304e6a/lessons/f758c44c-5e40-4e01-93b5-1a82aa4e044f/concepts/16cf4a78-4fc7-49e1-8621-3450ca938b77) for the required version and installation scripts.

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF

Then download and run the [term 2 simulation](https://github.com/udacity/self-driving-car-sim/releases), select the first one (project 1/2 EKF and UKF) and press start for testing.

![akf simulation](./ekf.png)

Red circles are lidar and blue circles are radar measurements. Green markers are the estimated position of the moving vehicle. Extended Kalman filter is very effective here estimating the position of the vehicle by reducing the measurement noise.