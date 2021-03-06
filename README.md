# simple_web_teleop


## requirements 
Install all dependencies with:

`rosdep install --from-paths src/simple_web_teleop -y -r`

or install manual:

### ROS bridge 

`sudo apt install ros-melodic-rosbridge-suite`

`roslaunch rosbridge_server rosbridge_websocket.launch`

### ROS web video server
`sudo apt install ros-melodic-web-video-server`

`rosrun web_video_server web_video_server`

### ROS Web Server (roswww) 

roswww is a lightweight web server package

Github: https://github.com/tork-a/roswww
ROS Wiki: http://wiki.ros.org/roswww

`sudo apt install ros-melodic-roswww`

`roslaunch roswww roswww.launch`


## Usage

`roslaunch simple_web_teleop simple_web_teleop.launch`

With roswww the default pre-configured port for the web server is 8085.

The server automatically provides access to files in a 'www' folder of each package (if this folder exists)
e.g.
 `http://ROSHOST:8085/simple_web_teleop/index.html`

(where `ROSHOST` is the IP or hostname of your robot)
