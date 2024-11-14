This is a basic setup for controlling a sitl drone inside gazebo simulator

start by running
 
`pip install -r requirments.txt`

start a sitl drone using your cordinates ie `latitude=42` & `longitude=-74`

`dronekit-sitl copter --home=40.68593813190999,-74.09225693035503,0,180`

start mavproxy and connect it to sitl drone on port 5760 and setup udp port 14550 and 14551 for mission planner

`mavproxy.py --master tcp:127.0.0.1:5760 --out udp:127.0.0.1:14551 --out udp:127.0.0.1:14550`

