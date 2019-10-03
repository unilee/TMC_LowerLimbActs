## Data collection for draft paper
These pages hold original data collected for experiments reported in our paper entitled 

_A novel adaptive and on-line IMU-based locomotion activity classification method using a triplet Markov model_

It also contains results for each subject, results not reported in the draft due to a lack of space.

### Data

The folder 'Data' includes all the experiments involved in the paper, for both training and testing data, it uses Matlab format. In each data file, there are two structs (_footStatic_ and _footMotion_) of the sensor readings, one is a short period with no movement and another one is a longer period with the four considered activities. The struct members are
 - time, in second
 - Accel_WideRange(acceleration), in m/s^2
 - Gyro (angular rate), in deg/s
 - Magnetic
 - Quat9DOF_WideRange, quaternion
    
Other useful information is also included in the file:
 - label, the ground truth of activity
 - switchLabel, the ground truth of activity switch, the first column represents previous activity, the second column represents the current activity.
  - lastRoundStartIndex, the start index of the second section in the experiment, relative to footMotion struct only.

### Results

The pdf file **dataexplanation** details the experiments of training and testing. The basic information of each subject is illustated there, and the results of the proposed adaptive on-line algorithm for each subject are also displayed.

### Citation

**If you would like to use this data, please cite one of the following references:**

[*Article #1*](https://www.sciencedirect.com/science/article/pii/S0925231219309956): H. Li, S. Derrode and W. Pieczynski. An adaptive and on-line IMU-based locomotion activity classification method using a triplet Markov model. Neurocomputing, 2019, 362:94-105 https://doi.org/10.1016/j.neucom.2019.06.081

[*Article #2*](https://www.mdpi.com/1424-8220/19/19/4242/htm): H. Li, S. Derrode and W. Pieczynski. Lower Limb Locomotion Activity Recognition of Healthy Individuals Using Semi-Markov Model and Single Wearable Inertial Sensor. Sensors, 2019, 19(19): 4242 https://doi.org/10.3390/s19194242
