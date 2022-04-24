# Project 3 Phase 2

## Introduction 
This file includes python program solution for Project 3 for
UMD ENPM 661 Spring 2022 batch. The folders consists of python
program along with generated outputs as .mp4 files.
  
    This project will solve given path planning puzzel using A* algoritm
    in the given world map using ROS simulation.
	
#### These files are executable:

  * bot_controller.py

## Requirements

       ***Important*********************************************************************
       *Unzip the folder and copy the enpm661_ws folder in your home directory*
       *********************************************************************************
       

	
### Running code in ubuntu

Make sure that current working derectory is same as the directory of program
Open your .bashrc file and paste the 2 lines that are written below

"source ~/enpm661_ws/devel/setup.bash
 export GAZEBO_MODEL_PATH=/home/nisarg/enpm661_ws/src/rwa3_group/models:$GAZEBO_MODEL_PATH "
" 
In the second line change the name from nisarg to your pc name.

After you go use "cd ~/enpm661_ws" to enter the workspace

kindly run the below command

=> rosdep install --from-paths ./src --ignore-packages-from-source -y
=> cd ~/enpm661_ws/src 

Do catkin build

After that launch the cmd roslaunch rwa3_group rwa3.launch"
& "rosrun rwa3_group bot_controller"

Fist cmd will launch the world and second will ask for user input

########################################################################

****NOTE  - Always keep the start node 475 and 25 y and x coordinate accordingly.
The reson is that it will take any start input and give you the result but the coordinate for bot launch is fixed in the map world that are according y - 475, x - 25****

After the path is found and final image is displayed press q for program to continue

After that you can see the burger bot will move according to the given path

By doing so first the path will be found using A* on the 2D environment then once the optimal path is found the ros simulation will work can you can see the results on the gazebo

#######################################################################


### Troubleshooting ###
	Most of the cases the issue will be incorrect working derectory.
	Double check the path by typing **pwd** command in console
  	This will output the current working directory.
  	Check if it is same as the python file location.

	For issues that you may encounter create an issue on GitHub.
  
### Maintainers ###
 Nisarg Upadhyay(nisargupadhyay2@gmail.com)
 Abhinav garg (agarg125@umd.edu)

### Video of Part ###
https://drive.google.com/file/d/17W1a0oDpO3Vjon0TzlkszFXZ1HPVdyRD/view?usp=sharing
