# CMP9767M

# Launching the Simulation

* Simple environment single robot, and fake localisation:
 
      roslaunch bacchus_gazebo vineyard_demo.launch world_name:=vineyard_small

  The parameter is also the default, so can be launched also as

      roslaunch bacchus_gazebo vineyard_demo.launch

  The Gazebo simulator is on pause by default after launching so you need to press the 'play' button in the bottom toolbar of Gazebo to start the simulation.


* More complex environment with different plant stages:
 
      roslaunch bacchus_gazebo vineyard_demo.launch world_name:=<WORLD>

  with `<WORLD>` being one of `vineyard_small`, `vineyard_stage0`, `vineyard_stage1`, `vineyard_stage2`, `vineyard_stage3`, `vineyard_stage4`, or `vineyard_stage0_heightmap`.

* If you intend to run a real localisation system (e.g. amcl) based on maps then set `fake_localisation:=false`. 

