# Closed-Loop Glucose Control Simulation

Simulation project developed as part of my Master's thesis in Computer Science.

The goal of this project was to compare selected approaches to closed-loop glucose control using a simulation environment based on glucose-insulin dynamics and continuous glucose monitoring.

The project compares three control strategies:

- PID controller
- Model Predictive Control
- Reinforcement Learning controller

## Project overview

Type 1 diabetes treatment requires continuous monitoring of glucose levels and appropriate insulin dosing. Closed-loop glucose control systems aim to automate part of this decision-making process by adjusting insulin delivery based on sensor data.

This project focuses on simulating and comparing different control algorithms in a simplified environment. The simulation includes glucose-insulin dynamics, CGM readings with delay and noise, insulin infusion and controller responses under different scenarios.

## Implemented approaches

### PID Controller

A classical feedback control method based on proportional, integral and derivative components.  
The controller reacts to CGM glucose values and adjusts insulin infusion according to the difference between the current glucose level and the target value.

### Model Predictive Control

A predictive control approach that uses a model of glucose-insulin dynamics to estimate future glucose behaviour and select insulin delivery decisions.

### Reinforcement Learning

A learning-based approach where an agent learns insulin dosing decisions through interaction with the simulated environment.  
The project uses an actor-critic style neural network approach for continuous insulin dosing.

## Evaluation metrics

The controllers were compared using metrics related to glucose control quality, including:

- Time in Range
- Time Below Range
- Time Above Range
- Mean glucose level
- Mean absolute error from target glucose
- Minimum and maximum glucose values
- Number of hypo- and hyperglycaemia episodes
- Total insulin delivered
- Reaction time after glucose deviation
- Glucose variability

## Repository contents

```text
closed-loop-glucose-control-simulation/
│
├── 1.ipynb      # Main simulation notebook
├── mag.pdf      # Master's thesis document
├── README.md    # Project description
└── .gitignore
```

## Technologies

- Python
- Jupyter Notebook
- NumPy
- pandas
- Matplotlib
- PyTorch
- Control algorithms
- Reinforcement Learning
- Simulation modelling

## Thesis document

The full thesis document is available in this repository:

[mag.pdf](mag.pdf)

## Important note

This project is a simulation created for academic and educational purposes.  
It is not a medical device and must not be used for real insulin dosing decisions.

## Author

Oliwia Groszek  
MSc in Computer Science
