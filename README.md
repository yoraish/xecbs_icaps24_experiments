# xECBS ICAPS 2024 Experimental Setup and Results
The experimental setup and results for the paper "Accelerating Search-Based Planning for Multi-Robot Manipulation by Leveraging Online-Generated Experiences."

In the paper, we presented results for two main experiments:
1. Motion planning in setups that **mimic the real-world scenarios** of multi-robot manipulation.
2. A **scalability analysis** -- low-clutter motion planning emphasizing the scalability of the proposed approach in terms of robot-robot interactions.

This repository includes the following files for each of the experiments:
1. A description file of the scene (robot placement locations) in the form of xacro files.
2. A MoveIt! file for the setup.
3. The start and goal configurations for the robots in each one of the trials.
   * Each trial includes information about the obstacles that were present in the scene during the test.
   * All start and goal configurations are in degrees.
4. The results of the experiments in the form of a CSV file.

Note 1: **trials had a 60-seconds runtime limit.** Therefore, all result rows with time larger than 60 seconds are considered as failures as well as those with values of `inf` or `-1` in the cost column.

Note 2: There might be an error in the scalability-10 files. The results may not match the problem descriptions.

Some files are not included in this repository (e.g., the URDF files of the robots, the STLs for visuals of obstacles, etc.), but those are either common and can be found online or are not necessary for the experimental setup (they were there just for looks).

