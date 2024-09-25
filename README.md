
# **AWS DeepRacer Student 2022: Rank 14**  
A reinforcement learning project demonstrating a high-ranking performance in AWS DeepRacer Student 2022.

## **Table of Contents**  
1. [Overview](#overview)  
2. [Reinforcement Learning and AWS DeepRacer](#reinforcement_learning)  
3. [Model Training](#model_training)  
4. [Track and Environment](#track_and_environment)   
5. [Rank and Achievements](#rank_and_achievements)   
6. [Inferences](#inferences)

---

## **Overview**<a name="overview"></a>  
Participation in AWS DeepRacer Student 2022 involved training a virtual car agent using reinforcement learning (RL) techniques. The car agent achieved a global rank of 14 in the competition. This repository provides insights into the training process, track-specific adjustments, and the final outcomes.

This project aims to provide the reward function that was used to train the car agent.

---

## **Reinforcement Learning and AWS DeepRacer**<a name="reinforcement_learning"></a>  
Reinforcement Learning (RL) is a type of machine learning where an agent learns to make decisions by performing actions in an environment and receiving rewards based on the success of those actions.

In AWS DeepRacer, the agent (a virtual car) is trained to complete laps on a simulated track as quickly as possible, while avoiding obstacles and staying within boundaries. The agent's learning process is guided by a **reward function** that encourages desired behavior, such as staying on the track or following the optimal racing line.

### **PPO Policy**  
The **Proximal Policy Optimization (PPO)** algorithm, developed by OpenAI, was used for training the car agent. PPO balances exploration (testing new strategies) and exploitation (relying on known strategies), resulting in stable and efficient learning.

By repeatedly running simulations, the car learns how to maximize the reward through trial and error. The final model showed significant improvement on the chosen track, enabling the agent to perform competitively.

---

## **Model Training**<a name="model_training"></a>  
The training was done using the PPO algorithm within AWS DeepRacer's cloud environment. The key steps involved in training include:

1. **Defining the Track:** The track selected for training was [insert track name] (image below), and the reward function was customized to encourage optimal lap times while avoiding penalties for going off-track.
   
2. **Training Process:**  
    - Multiple episodes were run to train the model on different segments of the track.  
    - The reward function was fine-tuned to incentivize aggressive cornering without compromising stability.  
    - Hyperparameters like learning rate and discount factor were adjusted for better performance.

---

## **Track and Environment**<a name="track_and_environment"></a>  
The track used for training was designed to test the car's ability to handle sharp turns, variable straightaways, and elevation changes. The environment setup focused on:

- **Track Layout:** Featuring tight corners and high-speed sections that challenge the balance between speed and control.
- **Simulation Conditions:** Variability in track conditions was introduced to ensure the model generalizes well to different race environments.

![Track Image](https://raw.githubusercontent.com/ishanmitra/aws-deepracer-student/refs/heads/main/images/track_waypoints.png)

---

## **Rank and Achievements**<a name="rank_and_achievements"></a>  
A rank of 14 was achieved in the AWS DeepRacer Student competition. Below are screenshots of the ranking and the certificate earned for participation:

![Ranking](https://raw.githubusercontent.com/ishanmitra/aws-deepracer-student/refs/heads/main/images/rank.png)

![Certificate](https://raw.githubusercontent.com/ishanmitra/aws-deepracer-student/refs/heads/main/images/Certificate_AWSInt.png)

---

## **Inferences**<a name="inferences"></a>  
The final model produced competitive lap times and was able to generalize across multiple test scenarios. The use of PPO allowed the agent to make efficient decisions, balancing speed and accuracy on the track.

The following insights were drawn from the experiment:
1. **Aggressive cornering strategies** helped improve lap times.
2. **Fine-tuning the reward function** had a significant impact on performance, particularly in penalizing off-track behavior.
