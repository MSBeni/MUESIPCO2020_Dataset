# MUESIPCO2020_Dataset
<h4> a reliable dataset,leveraging specific set of four optical cameras to provide ground truth with millime- ters accuracy. The introduced dataset consists of RSSI values col- lected from five BLE sensors together with synchronized Inertial Measurement Unit (IMU) signals from the target’s mobile device.</h4>


![Roadmap](Results/results.png)

## Dataset
Given the recent surge of interest on location-based services via BLE beacons, lack of a dataset with ground truth (actual labels) can be a significant obstacle for advancement of BLE-based indoor tracking/localiztion algorithms and research reproducibility. The paper takes a first step towards this goal and introduces the IoT-TD dataset, where the “Ground Truth Trajectories” are recorded in a synchronized fashion with the RSSI values together with IMU sensor measurements obtained, synchronously, from the moving target’s hand-held device. All three components of the dataset are time-stamped and pre-processed being available publicly for future BLE and PDR tracking algorithmic developments.

## Pre-Training
Our pre-training dataset consists of 94323 frontal view chest X-ray images for common thorax diseases. This dataset is extracted from the NIH Chest X-ray dataset available online for public access <a href="https://nihcc.app.box.com/v/ChestXray-NIHCC/folder/36938765345">here</a>. Chest X-ray14 dataset originally contains 112120 X-ray images for 14 thorax abnormalities. This dataset also contains normal cases without specific findings in their corresponding images.<br>To reduce the number of categories, we classified these 15 groups into 5 categories based on the underlying relations between the abnormalities in each disease. The first four groups are dedicated to No findings, Tumors, Pleural diseases, and Lung infections categories. The fifth group encompasses other images without specific relations with the first four groups.
We then removed 17797 cases with multiple labels (appeared in more than one category) to reduce the complexity and downscaled all images from (1024,1024) to (224,224).

### Experiment Setup
The experimental environment used to construct the IoT-TD dataset is a 3.5 meters to 3.5 meters area. Five BLE modules are used together with the built-in IMU sensor measurements of the user’s mobile device, recorded synchronously with RSSI values.  



