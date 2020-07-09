## Installing and running a TurtleBot3 simulator

### 1. To install the dependent packages, start from your catkin_ws/src folder:
``` cd ~/catkin_ws/src/ ``` 

 ``` git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git ``` 
 
``` git clone https://github.com/ROBOTIS-GIT/turtlebot3.git ```

``` cd ~/catkin_ws && catkin_make ```

![](images/1.PNG)

#### TurtleBot3 has three models, add this line ` export TURTLEBOT3_MODEL=burger ` at the bottom of the file to go with "burger model" after you enter the command:
``` gedit ~/.bashrc ```

![](images/3.PNG)

Save and quit the file.

#### reload .bashrc so that you do not have to log out and log back in.
``` source ~/.bashrc ```

### 2. to download the TurtleBot3 simulation files.
``` cd ~/catkin_ws/src/ ```

``` git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git ```

``` cd ~/catkin_ws && catkin_make ```

![](images/2.PNG)

### 3. To launch the virtual robot using Gazebo

#### First,launch TurtleBot3 in an empty environment by : 
` source devel/setup.bash `

``` roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch ```

![](images/4.PNG)

#### Your screen should look like this:

![](images/result.PNG)

 ### 4. To control the movement of your TurtleBot:
 In a new terminal tap: 
 
` source devel/setup.bash `
 
 ` roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch `

![](images/movement.PNG)

#### Use the buttons displayed in the terminal to control the movement.


