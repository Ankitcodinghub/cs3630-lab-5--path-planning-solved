# cs3630-lab-5--path-planning-solved
**TO GET THIS SOLUTION VISIT:** [CS3630 Lab 5- Path Planning Solved](https://www.ankitcodinghub.com/product/cs-3630-introduction-to-robotics-and-perception-solved-4/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;127067&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3630 Lab 5- Path Planning Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
LAB 5: PATH PLANNING

The objective of this lab is to implement and test robot path planning capabilities, specifically the RRT algorithm. You will first implement the RRT algorithm, then apply it to drive a 2D robot in the WeBots simulation environment from start to goal configurations. In this lab, we assume that the obstacles and map are known ahead of time.

All the code you have to implement is in the controllers/rrt_controller subfolder. Specifically, look for the files controllers/rrt_controller/map.py and controllers/rrt_controller/rrt.py.

Part 1 – Basic RRT

Please complete the following helper functions in controllers/rrt_controller/map.py.

• is_inbound()

• is_inside_obstacle()

• node_generator()

• step_from_to()

To test these helper functions, we have given you a local autograder. This should be much faster to run locally than on Gradescope. To run the autograder, navigate to the

controllers/rrt_controller subfolder, then run python3 autograder.py helpers

Afterwards, complete the RRT method in rrt.py, which handles the main loop of the algorithm. We provide code to limit the maximum number of nodes generated and terminate the loop once a path to goal has been found. Use your helper functions to implement the rest of RRT. Again, you can test this locally with python3 autograder.py rrt

Once the above steps are complete, you can validate that your RRT algorithm works with the

WeBots simulator. (More detailed steps are on the next page.)

1. Open rrt_controller.py and ensure that the MAP_NAME constant at the top is set to the map you would like to test on. The maps are named maze1, maze2, and maze3 (e.g. “./maps/maze2.json”). A working implementation should work on all three maps.

2. Launch WeBots. Click File &gt; Open World, then navigate to the “worlds” subfolder. Open the .wbt file which matches the MAP_NAME from step 1.

3. A GUI window should appear which shows your RRT code running in a simple 2D approximation of the world to find a path. Then, the robot in WeBots should start moving along this path.

a. We recommend selecting the “DEF e-puck Robot” object via the sidebar in the topleft of the WeBots screen. This will allow you to see the coordinate frame of the robot while it moves through the maze.

b. Note that the 2D GUI window should automatically close after the robot is done moving.

Figure 1. The WeBots world maze2 with the coordinate frame of the e-puck robot selected.

Part 2 – Path Smoothing

Once again, you can test your implementation with the WeBots simulator, which will follow the same procedure detailed above.

To test this part, you can use the same local autograder. This should be much faster to run locally than on Gradescope. To run the autograder, navigate to the controllers/rrt_controller subfolder, then run python3 autograder.py smoothing

Grading: Your grade will come from the autograder running your code on the three maps you are given, plus three hidden maps which are different than the hidden ones.

The exact point breakdown is as follows:

Helpers

is_inbound() 5 pts

is_in_obstacle() 5 pts

step_from_to() 10 pts

Full RRT implementation

RRT, autograded with 6 maps (3 hidden), 10 points per solved map 60 pts

Path Smoothing

Path smoothing, autograded with unsmoothed trajectories given 20 pts

Submission: Submit the files rrt.py and map.py to Gradescope. If you relied significantly on any external resources to complete the lab, please reference these in the submission comments.
