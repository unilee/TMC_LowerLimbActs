# TMC-HIST-based adaptive on-line recognition method for lower limb activities
This is a multi-activity recognition method that we publish in &lt;&lt;Signal Processing>> journal. 
## Data
The folder 'Data' includes all the experiments involved in the paper, for both training and testing data, the format is in matlab style. In each data file, there are two structs (footStatic and footMotion) of the sensor readings, one is a short period for no movement and another one for the four considered activities. The struct contains the memberships:
 - time, in second
 - Accel_WideRange(acceleration), in m/s^2
 - Gyro (angular rate), in deg/s
 - Magnetic
 - Quat9DOF_WideRange, quaternion
    
Other useful information is also included in the file:
 - label, the ground truth of activity
 - switchLabel, the ground truth of activity switch, the first column represents previous activity, the second column represents the current activity.
  - lastRoundStartIndex, the start index of the section section in the experiment, relative to footMotion struct only.
## Results
The .pdf file <<dataexplanation>> details the experiments of training and testing. The basic information of each subject is illustated there, and the results of the proposed adaptive on-line algorithm  for each subject are also displayed.
