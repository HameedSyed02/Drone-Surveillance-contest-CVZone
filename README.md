# Drone-Surveillance-contest-CVZone

HI I am Hameed . As the part of Drone-Surveillance-contest conducted by CVZone https://www.computervision.zone/dsc/. Here I implemented a car counter, my approach is by using yolov4 + deep sort model repo : https://github.com/theAIGuysCode/yolov4-deepsort

Training the Custum weights which to detect cars in the Drone Surveillance footage. The Custum weights file Trained Link : https://drive.google.com/file/d/1KSKVCgCILg6K5WWM2JAIlbPmXmgqnq_W/view?usp=sharing
 
I have made some code changes in Model files as of the purpose of the Contest. The OutPut is Shown Below

![alt text](https://github.com/HameedSyed02/Drone-Surveillance-contest-CVZone/blob/main/ss.png?raw=true)


Process To Implement
1: Download the yolov4 + deep sort repo:   https://github.com/theAIGuysCode/yolov4-deepsort
2: Downmoad The Custum Trained weights file : https://drive.google.com/file/d/1KSKVCgCILg6K5WWM2JAIlbPmXmgqnq_W/view?usp=sharing
3: Replace The modified code object_tracker.py with the Previous One in the repo
4: Move Weights file to ./Data/Custum-yolov4-car.weights
5: Move the Input video to ./Data/video/Drone.mp4

Follow the commands as below:  I recommand to use Anaconda 
conda env create -f conda-gpu.yml
conda activate yolov4-gpu
python save_model.py --model Custum-yolov4-car     (Load The Custum weights File)
python object_tracker.py --video ./data/video/Drone.mp4 --output DroneOutput.avi --model Custum-yolov4-car

The Output Video will be in the main diretory

I hope you Like it | Have a Great Day !  
