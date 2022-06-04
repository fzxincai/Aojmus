1.You can run the 'download_videos. m' in  "MoajCF" to get the OTB - 50, the OTB - 100, or directly to go to http://cvlab.hanyang.ac.kr/tracker_benchmark/datasets.html to download.
2.Change the video path under "run_tracker.m" in "MoajCF", which is the saved OTB data set path. Then run, you can get the accuracy and frame rate of each video sequence.

If you want to get the comparison results of this algorithm and other algorithms, you need to do the following configuration:
a. Download "tracker_benchmark_v1.0" from http://cvlab.hanyang.ac.kr/tracker_benchmark/benchmark_v10.html and perform simple configuration, the tutorial can be searched online;
b. Change "configTrackers.m" in "tracker_benchmark_v1.0\util" to add the algorithm to be compared;
c. Change "configSeqs.m" in "tracker_benchmark_v1.0\util", select the video sequence to be tested, and pay attention to the save path of the video sequence;
d. Run "main_running.m" in "tracker_benchmark_v1.0" to get the ".mat" file output by each algorithm in b. Then run "perfPlot.m" and "drawResultBB.m" respectively to get the curve graph and tracking results of each video sequence.

We provide the source code of "MoajCF", the ".mat" file output by the 8 algorithms in the paper in "tracker_benchmark_v1.0", and the line graph data in Figure 4 in the paper. ".mat" is contained in the "Results_OPE_CVPR13" folder and can be used directly in "tracker_benchmark_v1.0\results"After configuring "tracker_benchmark_v1.0", you can directly run and display the results. This article only compares the "OPE" of the algorithm. The 85 video sequences selected are as follows（where Skating2 and Jogging contain two video sequences respectively）:

'Basketball','Biker','BlurBody','BlurCar2','BlurFace','BlurOwl','Bolt','Box','Car1','Car4','CarScale','Couple','Crowds','David','Diving','DragonBaby','Dudek','Football','Freeman4','Girl','Human3','Human4','Human6','Human9','Ironman','Jump','Jumping','Liquor','MotorRolling','Panda','RedTeam','Singer2','Skating1','Skating2','Skiing','Soccer','Surfer','Sylvester','Trellis','Walking','Walking2','Woman','Bird2','BlurCar1','BlurCar3','BlurCar4','Board','Bolt2','Boy','Car2','Car24','Coke','Coupon','Crossing','Dancer','Dancer2','David2','David3','Dog','Dog1','Doll','FaceOcc1','Fish','FleetFace','Football1','Freeman1','Girl2','Gym','Human2','Human5','Human7','Human8','Jogging','Lemming','Man','Mhyang','MountainBike','Rubik','Skater2','Subway','Suv','Trans','Twinnings'.

