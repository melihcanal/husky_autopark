1. Start the autopark simulation for Husky:

	roslaunch husky_gazebo husky_autopark.launch

2. Start the Clearpath-configured rviz visualizer:

	roslaunch husky_viz view_robot.launch

3. Start the gmapping demo with any of these:

	roslaunch husky_navigation gmapping_dijkstra_dwa.launch (uses move_base library with global planner dijkstra and local planner dwa)
	
	roslaunch husky_navigation gmapping_dijkstra_teb.launch (uses move_base library with global planner dijkstra and local planner teb)
	
	roslaunch husky_navigation gmapping_astar_dwa.launch (uses move_base library with global planner a* and local planner dwa)
	
	roslaunch husky_navigation gmapping_astar_teb.launch (uses move_base library with global planner a* and local planner teb)

4. To save the generated map, you can run the map_saver utility:

	rosrun map_server map_saver -f <filename>
