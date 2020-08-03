# simple_web_teleop


## requirements 

### ROS bridge 

`sudo apt install ros-melodic-rosbridge-suite`

`roslaunch rosbridge_server rosbridge_websocket.launch`



### ROS Web Server (roswww) 

roswww is a lightweight web server package

Github: https://github.com/tork-a/roswww
ROS Wiki: http://wiki.ros.org/roswww

`sudo apt install ros-melodic-roswww`

`roslaunch roswww roswww.launch`


## Usage

With roswww the default pre-configured port for the web server is 8085.

The server automatically provides access to files in a 'www' folder of each package (if this folder exists)
e.g.
 `http://ROSHOST:8085/simple_web_teleop/index.html`

(where `ROSHOST` is the IP or hostname of your robot)
