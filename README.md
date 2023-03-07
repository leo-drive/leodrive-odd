# leodrive-odd



| Name             | Category   | Use Case                                                               | Description                                                                      | Default value             | Result       |
|------------------|------------|:-----------------------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------|--------------|
| UC-	001-0001     | Lane keep  | Normal driving                                                         | Keep the lane                                                                    | Parameters                | WORKS FINE   |
| UC-	001-0002     | Lane keep  | Following the vehicle in front                                         | Drive at a constant speed                                                        |                           | WORKS FINE   |
| UC-	001-0003     | Lane keep  | Stop of the vehicle in front during following it                       | Follow in the same lane                                                          |                           | WORKS FINE   |
| UC-	001-0004     | Lane keep  | Cutting-in during normal driving                                       | Keep a certain distance from the vehicle in front                                |                           | WORKS FINE   |
| UC-	001-0005     | Lane keep  | Cutting-out of the vehicle in front during following it                | Follow in the same lane                                                          |                           | WORKS FINE   |
| UC-	001-0006     | Lane keep  | Stop due to the detection of the crossing pedestrian on the crosswalk  | Stop at a safe distance from the vehicle in front after it stopped"              |                           | WORKS FINE   |
| UC-	001-0007     | Lane keep  | Driving at crosswalk                                                   | Follow in the same lane                                                          |                           | WORKS FINE   |
| UC-	001-0008     | Lane keep  | Driving over speed bump                                                | Keep the distance from the vehicle in front after it cut in                      |                           | WORKS FINE   |
| UC-	001-0009     | Lane keep  | Stop due to the obstacle on the same lane                              | Follow in the same lane                                                          | launch_speed_bump: true   | WORKS FINE   |
| UC-	001-0010     | Lane keep  | Swerving around the static object                                      | Drive at a given speed after the vehicle in front cut out                        |                           | WORKS FINE   | 
| UC-	001-0011     | Lane keep  | Stop due to Stop Sign                                                  | Follow in the same lane                                                          | avoidance/pedestrian: true | WORKS FINE   |
| UC-	001-0012     | Lane keep  | Driving in roundabout                                                  | Detect the crossing pedestrian on the crosswalk and stop at a safe distance      |                           | WORKS FINE   |
| UC-	001-0013     | Lane keep  | Driving in fourway                                                     | Follow in the same lane                                                         |                           | WORKS FINE   |

#### How to run the tests?

`ros2 launch scenario_test_runner scenario_test_runner.launch.py sensor_model:=golf_sensor_kit vehicle_model:=golf_vehicle \
scenario:=/home/user-name/scenario-folder/t4v2.yaml\
architecture_type:=awf/universe launch_rviz:=false launch_autoware:=true`
