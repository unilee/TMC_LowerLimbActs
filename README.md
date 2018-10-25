# TMC-HIST-based adaptive on-line recognition method for lower limb activities
This is a multi-activity recognition method that we publish in &lt;&lt;Signal Processing>> journal. 
## Data
The folder 'Data' includes all the experiments involved in the paper, for both training and testing data, the format is in matlab style. In each data file, there are two structs (footStatic and footMotion) of the sensor readings, one is a short period for no movement and another one for the four considered activities. The struct contains the memberships:
- time,
- Accel_WideRange(acceleration), in m/s^2
- 
