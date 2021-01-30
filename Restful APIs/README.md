# LGSVL RESTful API

## Main Page
http://Simplexity-Lab/LGSVL
## Command API [POST]
### Load Scene
http://Simplexity-Lab/LGSVL/LoadScene?scene=<scene_name>
### Set weather effect
**1. Nice weather**  
http://Simplexity-Lab/LGSVL/Control/Weather/Nice  
**2. Rain**  
2.1. Light Rain  
http://Simplexity-Lab/LGSVL/Control/Weather/Rain?rain_level=Light  
2.2. Moderate Rain  
http://Simplexity-Lab/LGSVL/Control/Weather/Rain?rain_level=Moderate  
2.3. Heavy Rain  
http://Simplexity-Lab/LGSVL/Control/Weather/Rain?rain_level=Heavy  
**3. Fog**  
3.1. Light Fog  
http://Simplexity-Lab/LGSVL/Control/Weather/Fog?fog_level=Light  
3.2. Moderate Fog  
http://Simplexity-Lab/LGSVL/Control/Weather/Fog?fog_level=Moderate  
3.3. Heavy Fog  
http://Simplexity-Lab/LGSVL/Control/Weather/Fog?fog_level=Heavy  
**4. Wetness**  
4.1. Light Wetness  
http://Simplexity-Lab/LGSVL/Control/Weather/Wetness?wetness_level=Light  
4.2. Moderate Wetness  
http://Simplexity-Lab/LGSVL/Control/Weather/Wetness?wetness_level=Moderate  
4.3. Heavy Wetness  
http://Simplexity-Lab/LGSVL/Control/Weather/Wetness?wetness_level=Heavy  

### Set time of day
**5. Time of Day**  
5.1. Morning  
http://Simplexity-Lab/LGSVL/Control/TimeOfDay?time_of_day=Morning  
5.2. Noon  
http://Simplexity-Lab/LGSVL/Control/TimeOfDay?time_of_day=Noon  
5.3. Evening  
http://Simplexity-Lab/LGSVL/Control/TimeOfDay?time_of_day=Evening  
### Agents control
**6. NPC Vehicle**  
6.1. NPC Vehicle Switch Lane  
http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Left_Lane&which_car=Sedan

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Right_Lane&which_car=Sedan

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Current_Lane&which_car=Sedan

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Left_Lane&which_car=SUV

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Right_Lane&which_car=SUV

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Current_Lane&which_car=SUV

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Left_Lane&which_car=Jeep

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Right_Lane&which_car=Jeep

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Current_Lane&which_car=Jeep

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Left_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Right_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Current_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Left_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Right_Lane&which_car=SchoolBus

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Current_Lane&which_car=SchoolBus

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Left_Lane&which_car=BoxTruck

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Right_Lane&which_car=BoxTruck

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleSwitchLane?which_lane=Current_Lane&which_car=BoxTruck

6.2. NPC Vehicle Maintain Lane

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Left_Lane&which_car=Sedan

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Right_Lane&which_car=Sedan

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Current_Lane&which_car=Sedan

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Left_Lane&which_car=SUV

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Right_Lane&which_car=SUV

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Current_Lane&which_car=SUV

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Left_Lane&which_car=Jeep

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Right_Lane&which_car=Jeep

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Current_Lane&which_car=Jeep

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Left_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Right_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Current_Lane&which_car=Hatchback

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Left_Lane&which_car=SchoolBus

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Right_Lane&which_car=SchoolBus

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Current_Lane&which_car=SchoolBus

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Left_Lane&which_car=BoxTruck

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Right_Lane&which_car=BoxTruck

http://Simplexity-Lab/LGSVL/Control/Agents/NPCVehicle/NPCVehicleMaintainLane?which_lane=Current_Lane&which_car=BoxTruck

6.2. NPC Vehicle Stop On Lane

**7. Pedestrians**  
7.1. Pedestrian walk on left lane  
http://Simplexity-Lab/LGSVL/Control/Agents/Pedestrians/WalkRandomly?which_lane=Left_Lane  
7.2. Pedestrian walk on right lane  
http://Simplexity-Lab/LGSVL/Control/Agents/Pedestrians/WalkRandomly?which_lane=Right_Lane  
7.3. Pedestrian walk on current lane  
http://Simplexity-Lab/LGSVL/Control/Agents/Pedestrians/WalkRandomly?which_lane=Current_Lane  

### Objects control
**8. Traffic Light**  
http://Simplexity-Lab/LGSVL/Control/ControllableObjects/TrafficLight  
## Status API [GET]
### EGO Vehicle Data
**1. Get Collision Information**  
http://Simplexity-Lab/LGSVL/Status/CollisionInfo  
**2. EGO Vehicle Status**  
2.1. Speed  
http://Simplexity-Lab/LGSVL/Status/EGOVehicle/Speed  
2.2. Position  
http://Simplexity-Lab/LGSVL/Status/EGOVehicle/Position  
### Sensors Data
**3. GPS Data**  
3.1. Latitude  
http://Simplexity-Lab/LGSVL/Status/GPS/Latitude  
3.2. Longitude  
http://Simplexity-Lab/LGSVL/Status/GPS/Longitude  
3.3. Northing  
http://Simplexity-Lab/LGSVL/Status/GPS/Northing  
3.4. Easting  
http://Simplexity-Lab/LGSVL/Status/GPS/Easting  
3.5. Altitude  
http://Simplexity-Lab/LGSVL/Status/GPS/Altitude 
