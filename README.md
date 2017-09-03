# CarND2-P2 Unscented Kalman Filter

## Description

**This my 2nd project result of Udacity self-driving car nanodegree (CarND) term 2. It's required to combine two types of sensing data, lidar and radar, to localize object using unscented Kalman filter (UKF). A simulator is provided to visualize sensing data and UKF localization result.**

**The following demonstrates UKF localization result and measurement data in action :** 

* Blue circle : radar measurement
* Red circle : laser measurement
* Green circle : computed UKF localization

![alt text][image1]

* Udacity self-driving car nanodegree (CarND) :

  https://www.udacity.com/course/self-driving-car-engineer-nanodegree--nd013
  
* Udacity self-driving car nanodegree term 2 simulator :

  https://github.com/udacity/self-driving-car-sim/releases/

The goals / steps of this project are the following:

[//]: # (Image References)
[image1]: ./images/ukf_1.gif

* The measurement data receiving and connection to simulator is in C++ file `./src/main.cpp`.

* The Unscented Kalman filter initialization, predict and update is called in C++ file `./src/ukf.cpp`.

* Fuction to calculate RMSE used for evaluation of localization quality is in C++ file `./src/tools.cpp`.

## Usage
* `mkdir build` 
* `cd build`
* `cmake ..`
* `make`
* `./UnscentedKF`
* Download simulator `term2_sim.app` (if in OSX) and open it. Click `play!` bottom, select Project 1/2: EKF and UKF, and press `Start` bottom to start.

## Unscented Kalman Filter (UKF)

Kalman filter is a typical technique used to fuse multiple sensing data and get a more accurate result (state) based on linear assumption and Bayes rule. 
Unlike (extended) Kalman filter which assumes measurement to be linear, unscented Kalman filter can be applied to both linear and nonlinear case. 




