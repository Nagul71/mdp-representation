# MDP REPRESENTATION

## AIM:
Write your aim here

## PROBLEM STATEMENT:
The problem involves managing a restaurant's seating arrangement during peak hours. The restaurant has limited seating capacity and receives a continuous stream of customers throughout the day. The goal is to maximize the restaurant's profit while ensuring customer satisfaction by efficiently managing the seating arrangements.

### Problem Description
Write your answer here

### State Space
The state space consists of three possible states:
```
Empty
Seated
Served
```

### Sample State
Seated

### Action Space
Action space conssists of 0 and 1

### Sample Action
A sample action could be 1

### Reward Function
Write your answer here

### Graphical Representation
Write your answer here

## PYTHON REPRESENTATION:
```py
mdp = {
    "Empty": {
         0 : [(0.6, "Empty", 0, False),(0.4, "Seated", 0, False)],
        1 : [(0.1, "Empty", 0, False),(0.9, "Seated", 0, False)]
    },
    "Seated": {
        0 : [(0.3, "Seated", 0, False),(0.7, "Empty", 0, False)],
        1 : [(0.7, "Seated", 0, False),(0.3, "Served", 1, True)]
    },
    "Served": {
        0 : [(1.0, "Served", 0, False)],
        1 : [(1.0, "Empty", 0, False)]
    }
}
```


## OUTPUT:
![image](https://github.com/Nagul71/mdp-representation/assets/118661118/5bc4536f-129e-4b71-b25e-bd234d3a0d04)


## RESULT:

The optimal strategy is to serve seated customers promptly, maximizing profit and ensuring efficient table turnover.

