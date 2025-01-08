---
layout: post
title: How far back shall we peer?
subtitle: Optimal air handling unit control leveraging extensive past observations
cover-img: /assets/img/Systeme-HVAC-scaled.jpeg
thumbnail-img: /assets/img/thumb_Informer_HVAC.jpg
share-img: /assets/img/path.jpg
tags: [Journal, HVAC control]
author: Rui Li and Zhengbo Zou
---
Heating, Ventilation, and Air Conditioning (HVAC) systems are at the heart of ensuring comfort and energy efficiency in buildings. Traditional Rule-Based Feedback Control (RBFC) systems, though simple and widely used, often lack adaptability to dynamic environments. Model Predictive Control (MPC) methods, while more advanced, require complex mathematical modeling and expert knowledge, posing significant barriers to design and optimization.  

In my latest research, I explored how Reinforcement Learning (RL) can revolutionize HVAC system optimization. Unlike traditional methods, RL offers adaptability and operates without the need for explicit models. However, RL's application to HVAC systems has been limited by challenges like sample inefficiency and suboptimal convergence, particularly when accounting for HVAC's delayed effects and prolonged thermal inertia.  

To overcome these challenges, I developed an innovative deep RL framework that integrates historical observations to enhance RL agent performance. At the core of this framework is a state-of-the-art Transformer model, which excels in capturing temporal patterns in HVAC data. This enables the creation of a more precise RL training environment.  

![Overall_architecture](https://Rui-29.github.io/assets/img/thumb_Informer_HVAC.jpg){: .mx-auto.d-block :}

In the framework, the process begins with stage a, where we collect HVAC variables from the BAS database. These variables are then preprocessed and categorized into states, actions, and rewards. Progressing to stage b, this structured dataset is employed to train the RL environment model. The model is designed to use both past and current state-action pairs to predict the subsequent step state and reward. In the final stage c, by considering both historical and immediate observations, our RL agent interacts with the environment and executes actions strategically to optimize the dual objectives of energy saving and thermal comfort.  

When tested on high-resolution, real-world HVAC datasets, the framework delivered satisfactory results:  
- **Prediction Accuracy**: Achieved a 30.5% and 35.8% improvement over Bi-LSTM and vanilla Transformer models, respectively.  
- **Energy Efficiency**: Realized a 35.3% reduction in electricity consumption compared to RBFC systems.  
- **Thermal Comfort**: Improved occupant comfort by 54.4%.  

These results demonstrate the transformative potential of integrating historical data and advanced machine learning techniques into HVAC system optimization. My research showcases how modern AI technologies, like RL and Transformers, can make our buildings smarter, more efficient, and more comfortable.  

Stay tuned for more updates on leveraging technology to drive sustainability and innovation in the built environment! 
