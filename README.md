# gazebo_world

This is a project I made for my Robotics Software Engineer Nanodegree from Udacity. It involves creating and visualizing a gazebo world with a personalized message displayed on the terminal. Gazebo is a simulator tool widely used in the robotics community. 

# Quickstart

## Requirement

Please install [**__ROS Kinetic__**](http://wiki.ros.org/kinetic/Installation "ROS Kinetic Installation") (choose your platform. I have used Ubuntu which is ROS supported)

## Building the project

Clone the project using `git clone https://github.com/sarkrishnan/gazebo_world.git` command

Navigate into the project folder `cd gazebo_world`

Create a build directory `mkdir build` and navigate into it `cd build` 

Use command `cmake ../` and then `make` to create the welcome_message gazebo plugin

Use command `export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:{path to the build folder}` to make the welcome_message gazebo plugin we created in the previous step visible to gazebo. Example code: `export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/myrobot/build` 


## Viewing the created Gazebo world

Navigate into the world folder `cd ../world` (Here I have assumed that we are still in the build folder)

Run the command `gazebo Project1_world`. It should open up the gazebo world and also display 'Welcome to Aravinda's world' in the terminal. The gazebo world will have couple of collapsed humanoid robots and a building structure with some tables. 

You have viewed the created Gazebo world successfully!

## Suggestions 

If you would like to change the welcome message, please navigate into script folder and make changes in the welcome_message.cpp

You can also create your own building and robot models and save them in the appropriate folder within model folder and also save the world from gazebo
