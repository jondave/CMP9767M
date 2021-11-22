# CMP9767M

# Launching the Simulation
* Simple environment _without_ obstacles, single robot, and fake localisation:
 
      roslaunch uol_cmp9767m_base thorvald-sim.launch obstacles:=false second_robot:=false fake_localisation:=true
      
  First two parameters are also the default, so can be launched also as

      roslaunch uol_cmp9767m_base thorvald-sim.launch fake_localization:=true
      roslaunch uol_cmp9767m_base thorvald-sim.launch fake_localisation:=true

* Simple environment _without_ obstacles, two robots, and fake localisation:

      roslaunch uol_cmp9767m_base thorvald-sim.launch obstacles:=false second_robot:=true fake_localisation:=true
* Realistic environment _with_ obstacles, single robot, and fake localisation (to truly show real navigation abilities, set `fake_localisation:=false` and provide your own map and robot localisation solution):
 
      roslaunch uol_cmp9767m_base thorvald-sim.launch obstacles:=true second_robot:=false fake_localisation:=true
* Realistic environment _with_ obstacles, two robots, and fake localisation (to truly show real navigation abilities, set `fake_localisation:=false` and provide your own map and robot localisation solution):
 
      roslaunch uol_cmp9767m_base thorvald-sim.launch obstacles:=true second_robot:=true fake_localisation:=true

  Also available as [video](https://youtu.be/MPMHnVZvOYo0).
* If you intend to run a real localisation system (e.g. amcl) based on maps then set `fake_localisation:=false`. If you want to use the provided simple map, you may additionally set `map_server:=true`.
