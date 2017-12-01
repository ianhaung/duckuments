# Anti-Instagram


## Part 1: System interfaces

Please note that for this part it is necessary for the system architect and software architect to check off before you submit it. Also note that they are busy people, so it's up to you to coordinate to make sure you get this part right and in time.

### Logical architecture

- Please describe in detail what the desired functionality will be. What will happen when we click "start"?

- Please describe for each quantity, what are reasonable target values. (The system architect will verify that these need to be coherent with others.)

- Please describe any assumption you might have about the other modules, that must be verified for you to provide the functionality above.

<!--
The above must have a check-off by the software architect:

System architect check-off: I, XXX, (agree / do not agree) that the above is compatible with system-level constraints.
-->

### Software architecture

- Please describe the list of nodes that you are developing or modifying.

- For each node, list the published and subscribed topics.

- For each subscribed topic, describe the assumption about the latency introduced by the previous modules.

- For each published topic, describe the maximum latency that you will introduce.

<!--
The above must have a check-off by the software architect:

Software architect check-off: I, XXX, (agree / do not agree) that the above is compatible with system-level constraints.
-->

## Part 2: Demo and evaluation plan


### Demo plan

Our demo plan consists of several different sub demos:
##### 2 duckiebots doing the lane-following demo
One of the duckiebots has the improved anti-instagram algorithm on it and the other duckiebot will run on the old version. With different light conditions in different parts of duckietown we try to show that the improved version performs better than the old version.

| **+**  | **-**  |
| :------------: | :------------: |
| One can see the improvement of the whole system.  | It is not obvious what the algorithm exactly does.  |
| It is very easy to understand  | One does not understand why the newer system works better.  |

*Important notes:*
- The two duckiebots only differ by the anti instagram algorithm. Everything else stays the same!
- If we don't have enough space we could run two similar videos in parallel. One of the old-version-duckiebot and one of the new-version-duckiebot. [Scenario II]

*Material needed [Scenario I]:*
1. Full version of duckietown
2. 2 Full working duckiebots

*Material needed [Scenario II]:*
1. Big video screen and computer attached

##### Interactive Live-Application of Anti-Instagram filtering.
The visitors can filter a static image with color filters and see an instant output image of the anti-instagram filter. This demo should show how accurate and powerful the anti-instagram algorithm is.

| **+**  | **-**  |
| :------------: | :------------: |
| It is very clear what the Anti-Instagram algorithm does  | It doesn't really attract people since it is very static |
| It is easy to understand  | It doesn't show whether the system has improved or not.  |

*Material needed:*
1. Touchscreen and computer unit
2. Program with ability to filter an image
3. Camera which films image
4. Second screen (?) with output image
##### Visualisation of the kMeans algorithm

We want to show on a screen

| **+**  | **-**  |
| :------------: | :------------: |
| It described the algorithm very clear in a short way. For people with interest is should be very understandable. | It is not very attractable. |
| It shows all the technical details (# of clusters, # of iterations, ...) | It is difficult to know what happens. Only for experts valuable. |

*Material needed:*
1. Screen with computer attached.
2. Visualisation of the kMeans algorithm


It should take a few minutes maximum for setup and running the demo.

- How do you envision the demo?

- What hardware components do you need?

### Plan for formal performance evaluation

- How do you envision the performance evaluation? Is it experiments? Log analysis?

In contrast with the demo, the formal performance evaluation can take more than a few minutes.

Ideally it should be possible to do this without human intervention, or with minimal human intervention, for both running the demo and checking the results.

<!--
Check-off by Duckietown Vice-President of Safety:

Duckietown Vice-President of Safety: I, (believe / do not believe) that the performance evaluation above is
-->
## Part 3: Data collection, annotation, and analysis

_Please note that for this part it is necessary for the Data Czars to check off before you submit it. Also note that they are busy people, so it's up to you to coordinate to make sure you get this part right and in time._

### Collection

- How much data do you need?

- How are the logs to be taken? (Manually, autonomously, etc.)

Describe any other special arrangements.

- Do you need extra help in collecting the data from the other teams?

### Annotation

- Do you need to annotate the data?

- At this point, you should have you tried using [thehive.ai](https://thehive.ai/) to do it. Did you?

- Are you sure they can do the annotations that you want?

### Analysis

- Do you need to write some software to analyze the annotations?

- Are you planning for it?

<!--
Check-off by Data Zars:

Data czars check-off: We, XXX and YYY, (believe / do not believe) that the plan above is well structured, and that we can provide the level of support requested.
-->