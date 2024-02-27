# MDP REPRESENTATION

## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways.

Text representation

Graphical representation

Python - Dictonary representation

## PROBLEM STATEMENT:
Developing a self-driving car system to navigate urban environments efficiently while adhering to traffic laws and ensuring passenger safety.

### State Space
The state space could include various factors such as:

Current location of the car.
Surrounding traffic conditions (density, speed, direction).
Pedestrian presence and behavior.
Traffic signals and signs.
Weather conditions.
Road conditions (lane markings, obstacles).
Passenger requests or destinations.
Time of day.

### Sample State
A sample state could be:

Current location: Intersection of Main Street and Elm Avenue.
Surrounding traffic: Moderate density, cars moving at 30 mph in all directions.
Pedestrian presence: Crossing at the crosswalk on Main Street.
Traffic signals: Green light for Main Street, red light for Elm Avenue.
Weather conditions: Clear skies.
Road conditions: Smooth asphalt with visible lane markings.
Passenger requests: Destination set to City Center.

### Action Space
The action space represents the decisions the self-driving car can make at each state:

Accelerate.
Decelerate.
Maintain current speed.
Change lanes.
Turn left/right.
Stop at traffic signal.
Yield to pedestrians.
Proceed through intersection.

### Sample Action
A sample action could be:

Accelerate to merge into the adjacent lane with faster-moving traffic.
Stop at the red traffic signal.
Yield to pedestrians crossing at the crosswalk.
Proceed straight through the intersection as the traffic signal turns green.

### Reward Function
The reward function incentivizes desirable behavior and penalizes undesirable actions:

Positive rewards for reaching the destination safely and efficiently.
Negative rewards for violating traffic laws (running red lights, speeding), causing accidents, or endangering pedestrians.
Additional rewards for passenger comfort and satisfaction.

### Graphical Representation

![Graphical ](https://github.com/SivaChandranR07/mdp-representation/assets/113497395/714e4b22-397d-4a7d-a22e-4fa418b8fcc8)

## PYTHON REPRESENTATION:
```
P = {
    0 : {
        0 : [(1.0, 0, 0.0, False)],
        1 : [(1.0, 1, 0.0, False)],
        2 : [(1.0, 2, 0.0, False)],
        3 : [(1.0, 0, 0.0, False)]
    },

    1 : {
        0 : [(1.0, 1, 0.0, False)],
        1 : [(1.0, 1, 0.0, False)],
        2 : [(0.8, 3, 0.0, False), (0.2, 1, 0.0, False)],
        3 : [(0.8, 0, 0.0, False), (0.2, 1, 0.0, False)]
    },

    2 : {
        0 : [(0.8, 0, 0.0, False), (0.2, 2, 0.0, False)],
        1 : [(0.8, 3, 0.0, False), (0.2, 2, 0.0, False)],
        2 : [(1.0, 2, 0.0, False)],
        3 : [(1.0, 2, 0.0, False)]
    },

    3 : {
        0 : [(0.8, 1, 0.0, False), (0.2, 3, 0.0, False)],
        1 : [(1.0, 3, 0.0, False)],
        2 : [(0.8, 4, 0.0, False), (0.2, 3, 0.0, False)],
        3 : [(0.8, 2, 0.0, False), (0.2, 3, 0.0, False)]
    },

    4 : {
        0 : [(0.8, 3, 0.0, False), (0.2, 4, 0.0, False)],
        1 : [(0.8, 5, 0.0, False), (0.2, 4, 0.0, False)],
        2 : [(0.8, 6, 0.0, False), (0.2, 4, 0.0, False)],
        3 : [(1.0, 4, 0.0, False)]
    },

    5 : {
        0 : [(1.0, 5, 0.0, False)],
        1 : [(1.0, 5, 0.0, False)],
        2 : [(0.8, 7, 1.0, True), (0.2, 5, 0.0, False)],
        3 : [(0.8, 4, 0.0, False), (0.2, 5, 0.0, False)]
    },

    6 : {
        0 : [(0.8, 4, 0.0, False), (0.2, 6, 0.0, False)],
        1 : [(0.8, 7, 1.0, True), (0.2, 6, 0.0, False)],
        2 : [(1.0, 6, 0.0, False)],
        3 : [(1.0, 6, 0.0, False)]
    },

    7 : {
        0 : [(1.0, 7, 0.0, True)],
        1 : [(1.0, 7, 0.0, True)],
        2 : [(1.0, 7, 0.0, True)],
        3 : [(1.0, 7, 0.0, True)]
    }
}
```
## OUTPUT:

![Screenshot 2024-02-23 095539](https://github.com/SivaChandranR07/mdp-representation/assets/113497395/f88ad48e-55a9-4d42-b203-639826c47ddf)

## RESULT:

Thus,developing a self-driving car system to navigate urban environments efficiently while adhering to traffic laws and ensuring passenger safety in reinforcement learning has been executed successfully.
