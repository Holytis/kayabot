# kayabot 
# Getting started
1.Clone the repo:
```
git clone https://github.com/Holytis/kayabot
```
2.Navigate to your workspace:
```
cd ~/kaya_ws
```
3.Update dependencies:
```
rosdep update
```
4.Install dependencies:
```
rosdep install --ignore-src --from-paths src -y -r
```
5.Compile
```
colcon build
```
# Operating Instructions
After you build, remember to source the proper install folder...
```
source ~/kaya_ws/install/local_setup.bash
```
And then run the launch file...
```
ros2 launch articubot_one launch_sim.launch.py use_sim_time:=true
```
After that run the this file to control robot
```
ros2 run articubot_one controller.py 
```
