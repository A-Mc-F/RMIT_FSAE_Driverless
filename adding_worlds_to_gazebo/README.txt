
RUNNING - once the below steps are completed
T1: roscore
T2: rosrun gazebo_ros gazebo

//launch the world

T3: roslaunch catvehicle skidpad_world.launch

//add the catvehicle

T4: roslaunch catvehicle catvehicle_spawn.launch robot:=catvehicle X:=0 Y:=20 \
yaw:=1.57079632679



STEPS to Complete

// copy provided skidpad.world file into /home/ubuntu/catkin_ws/src/catvehicle/worlds/skidpad.world
// copy provided skidpad_world.launch file to /home/ubuntu/catkin_ws/src/catvehicle/launch/skidpad_world.launch
// copy the provided "eufs_sim" folder to your Desktop

//to copy the files/folders, open them on git, click raw, then right-click and save to the sorresponding place.

cd ~/.gazebo/
cd models
mkdir skidpad
cd skidpad/

//make config file - copy contents from below

atom model.config  // i use atom text editor if you dont have a custom one change atom to gedit

// make sdf file - copy contents from below
atom model.sdf
mkdir meshes

// this command copies the contents of "eufs_description/meshes" into /skidpad/meshes"
cp -R /home/ubuntu/Desktop/eufs_sim/eufs_description/meshes/. ~/.gazebo/models/skidpad/meshes/


//Contents of model.config (dont include outer quotation marks)

"
<?xml version="1.0" ?>
<model>
    <name>skidpad</name>
    <version>1.0</version>
    <sdf version="1.6">model.sdf</sdf>
    <author>
        <name></name>
        <email></email>
    </author>
    <description></description>
</model>

"

//contents of model.sdf
<?xml version='1.0'?>
    <sdf version='1.6'>
        <model name='skidpad'>
    <link name='link'>
      <pose frame=''>-1.637 0 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-2.216 2.9131 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-3.867 5.3828 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-6.336 7.0330 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-9.25 7.6125 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-12.16 7.0330 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-14.63 5.3828 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-16.28 2.9131 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-16.86 0 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-16.28 -2.913 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-14.63 -5.382 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-12.16 -7.033 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-9.25 -7.612 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-6.336 -7.033 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-3.867 -5.382 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-2.216 -2.913 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>19.862 0 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>19.054 4.0612 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>16.754 7.5041 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>13.311 9.8046 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>9.25 10.612 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>5.1887 9.8046 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.7458 7.5041 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.7458 -7.504 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>5.1887 -9.804 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>9.25 -10.61 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>13.311 -9.804 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>16.754 -7.504 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>19.054 -4.061 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_blue.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>16.862 0 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>16.283 2.9131 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>14.632 5.3828 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>12.163 7.0330 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>9.25 7.6125 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>6.3368 7.0330 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>3.8671 5.3828 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>2.2169 2.9131 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 0 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>2.2169 -2.913 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>3.8671 -5.382 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>6.3368 -7.033 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>9.25 -7.612 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>12.163 -7.033 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-3.867 -5.382 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>14.632 -5.382 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>16.283 -2.913 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.745 7.5041 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-5.188 9.8046 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-9.25 10.612 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-13.31 9.8046 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-16.75 7.5041 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-19.05 4.0612 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-19.86 0 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-19.05 -4.061 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-16.75 -7.504 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-13.31  -9.80 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-9.25 -10.61 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-5.188 -9.804 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.745 -7.504 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_yellow.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 -9 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 -11 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 -9 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 -11 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 9 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 11 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 13 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 15 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 17 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 19 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 9 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 11 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 13 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 15 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 17 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 19 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.637 21 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.6375 21 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-0.55 21 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>0.55 21 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.783 1.4851 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>-1.783 -1.485 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.7837 1.4851 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
    <link name='link'>
      <pose frame=''>1.7837 -1.485 1 0 -0 0</pose>
      <collision name="collision">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </collision>
      <visual name="visual">
        <geometry>
          <mesh>
            <uri>model://skidpad/meshes/cone_big.dae</uri>
          </mesh>
        </geometry>
      </visual>
    </link>
  </model>
</sdf>
