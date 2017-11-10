# Hand_Gesture_Command

Hand Gesture Command allows a person to command BWI Segbot through hand gesture rather than traditional ways of 
user manual keyboard input.

Hand Gesture Command requires the running of the following nodes.
1. background_people_perception (git clone: https://github.com/utexas-bwi/bwi_experimental)
2. fri_object_following_creeper (git clone: https://github.com/JGOOSH/fri_object_following)

After running these two nodes, you can start the prgogram by run
"hand_gesture_command" 

How to Run: 
1. Download utexas-bwi library (if not installed). Git clone : https://github.com/utexas-bwi/bwi
2. Download background_people_perception (git clone: https://github.com/utexas-bwi/bwi_experimental)
3. Download fri_object_following_creeper (git clone: https://github.com/JGOOSH/fri_object_following)
4. Download this repo (git clone: https://github.com/JGOOSH/Hand_Gesture_Command/)
5. catkin_make
6. source devel/setup.bash
7. roslaunch bwi_launch segbot_v2.launch 
8. Localize the robot
9. Run background_pcl_perception: roslaunch pcl_perception background_people_detection_v2.launch
10. Run creeper: rosrun fri_object_following creeper
11. Run hand gesture command : rosrun hand_gesture_command hand_gesture_command

Created by Jamin Goo and Mehrdad Darraji

Hand Tracking implemention credit to http://simena86.github.io/blog/2013/08/12/hand-tracking-and-recognition-with-opencv/
	
Link to working demo: https://www.youtube.com/watch?v=8Fok6OR0DR8

* currently only support version 2 only. 
