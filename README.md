# MDP REPRESENTATION

## AIM:
To represent any one real-world problem in MDP form.

## PROBLEM STATEMENT:
A customer is planning to buy a product online. They have three websites to choose from: Option A, Option B, and Option C. The customer wants to select the best website based on their preferences and the associated rewards.

### Problem Description
choosing the best website to buy

### State Space
The state space consists of the different options available for the customer to choose from:
```
State 0: Website A
State 1: Website B
State 2: Website C
```

### Sample State
A sample state could be the customer currently considering website B.

### Action Space
The action space consists of the decisions the customer can make:
```
Action 0: Stay with the current option
Action 1: Switch to the next option
```

### Sample Action
A sample action could be the customer deciding to switch from Website A to Website B.

### Reward Function
```
The customer receives a reward of 0 for staying with the current option.
If the customer switches to the last option (Website C), they receive a reward of 1.
There are no intermediate rewards for other actions or states.
```

### Graphical Representation

![WhatsApp Image 2024-02-25 at 21 02 00_b9298ddd](https://github.com/Nagul71/mdp-representation/assets/118661118/8f6d90eb-32bc-488c-b66c-6136f15165f6)

```
Developed By:
Name : NAGUL K
Reg No : 212222230089


## PYTHON REPRESENTATION:
```py
P = {
    0:{
        0: [(1.0, 0, 0.0, True)],  
        1: [(1.0, 1, 0.0, True)]   
    },
    1:{
        0: [(1.0, 1, 0.0, True)],  
        1: [(1.0, 2, 1.0, True)]   
    },
    2:{
        0: [(1.0, 2, 0.0, True)],  
        1: [(1.0, 2, 0.0, True)]   
    }
}
```


## OUTPUT:

![Screenshot 2024-02-25 204439](https://github.com/Nagul71/mdp-representation/assets/118661118/8ab226d5-968f-4165-b900-fab5b5612d7b)


## RESULT:

Thus the given real world problem is successfully represented in a MDP form .

