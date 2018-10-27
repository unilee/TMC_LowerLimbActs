## Data collection for draft paper
These pages hold original data collected for experiments reported in our draft paper entitled 

_A novel adaptive and on-line IMU-based \\locomotion activity classification method \\using a triplet Markov model_

It also contains results for each subject, results noe reported in the draft due to a lack of space.

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
  - lastRoundStartIndex, the start index of the section section in the experiment, relative to footMotion struct only.

### Results

The pdf file **dataexplanation** details the experiments of training and testing. The basic information of each subject is illustated there, and the results of the proposed adaptive on-line algorithm for each subject are also displayed.
