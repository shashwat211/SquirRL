
# CS577 Introduction to Blockchain and Cryptocurrency: Project Code  

## Team Details:

**Team Name**: 29  
**Team Members**

| **Name**              | **Roll Number** |
| ----------------- | ----------- |
| Kunj Taneja   | 1801CS30    |
| Shashwat Mahajan      | 1801CS46    |
| Vanshika Srivastava  | 1801CS69    |

## Code Details

This is the implementation of the Single Agent part of paper *SquirRL: Automating Attack Discovery on Blockchain Incentive Mechanisms with Deep Reinforcement Learning* (https://arxiv.org/abs/1912.01798). Additionally, we have added the code for an additional GHOST protocol.

## Single Agent Part

We test 3 different chain rules: Bitcoin(longest chain rule), Ethereum(uncle block rule) and GHOST (heaviest sub-tree rule, this is our own implementation). 

### Basic Usage

In `\SingleAgent`,  run

```
python btc.py
python eth.py
python ghost.py
```

and you can train the RL agents and test them. 

### Main Files

`\SingleAgent\environment.py` 

The interactive environment for 3 different protocols. OpenAI gym type APIs. 

`\SingleAgent\btc.py` , `\SingleAgent\eth.py`, `\SingleAgent\ghost.py` 

The training and testing part of the RL agent for the Bitcoin/Ethereum/GHOST protocols. You can find more detailed comments of training in `\SingleAgent\btc.py`. 

`\SingleAgent\optimal_policy.py`

The implementation of *Optimal Selfish Mining*. We saved the policy in `optimal_policy.txt`. 
