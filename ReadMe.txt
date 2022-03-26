## ------------------------------------------------------------------------------------------
#                                       A* Algorithm
## ------------------------------------------------------------------------------------------

# Author: Jai Sharma (UID: 118160016) & Divyansh Agrawal (UID: 117730692)
# Course: ENPM661 - Planning for Autonomous Robots
# Assignment: Project 3 Phase 1

## ------------------------------------------------------------------------------------------

Goal: 
- Implementing A-Star Algorithm for a Rigid Robot

Work: 
- In this project, the A-Star algorithm has been implemented for a point robot. 
- A map of dimensions 400 * 250 is given which has multiple obstacles in it. 
- The user has to input the initial node [x,y] and the goal node [x,y] and then the algorithm solves for the path. 
- The file (A_Star_Algorithm.py) can be opened in any python editor and then run. 

Additonal Notes:
1) the program requires user to enter 4 inputs: Xi, Yi, Xg, Yg
	- the radius, step size and clearance is set to 1 unit each
	- the initial and final orientation of robot is set to 0 degrees
2) the program can take between 1 to 3 minutes to run. 
	- most test cases took about 6 minutes on my computer.
    	- the code prints the runtime for reference
3) there are a few bugs in the code, it's not entirely robust:
	- the map has a few hidden boundaries that act as an imaginary obstacle when the robot is looking for a path.
	- the boundaries might have arrived from defined obstacle spaces. 
	- this can be seen when user execute codes for start = (0,0), goal = (150,50)
	- the bug shall be fixed prior to Project 3 Phase 2 submission.
4) the plotted nodes are actually rounded nodes, hence the visualized path between nodes is made of increments of 1 in vertical and horizontal direction.

The A* algorithm performs as expected if not for the hidden boundaries.The video submissions are included. 
The 2 test cases that worked for our code are as follows:
	Test Case 1. start = (0,0), goal = (185,225)
	Test Case 2. start = (85,75), goal = (390,215)


## ------------------------------------------------------------------------------------------

For any questions regarding the implementation or running of the program, please contact dagrawa1@umd.edu.
Github: https://github.com/divyansh2681
Github: https://github.com/jaisharma10

## ------------------------------------------------------------------------------------------

References Used:
1. https://medium.com/@nicholas.w.swift/easy-a-star-pathfinding-7e6689c7f7b2