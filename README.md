This Jupyter notebook focuses on optimizing overbooking strategies for an airline, specifically dealing with the allocation of seats in main cabin and first class. Here's an overview of the various components and functionalities implemented in the notebook:

Setup and Initialization:
Introduction and Variables Definition: I provide a comprehensive description of the business scenario, including the types of tickets (main cabin and first class), the concept of overbooking, and the associated costs of upgrading passengers or denying boarding due to overbooking. Important variables like prices, sale probabilities, and the number of seats available in each class are defined.

Parameter Setup: I set up essential parameters such as the probabilities of ticket holders showing up, the prices for both classes under different conditions (high or low), and the overbooking limit. Arrays are also created to handle combinations of prices and sale probabilities effectively.

Modeling and Calculations:
Dynamic Programming Setup: A dynamic programming approach is used to model the problem. I initialize matrices to keep track of the value function and policy decisions (price selections) over a time horizon leading up to the flight departure. This setup helps in determining the optimal number of tickets to sell each day to maximize profits while minimizing costs related to overbooking.

Terminal Value Calculation: At the end of the planning horizon (flight departure), I calculate the terminal values for the value function matrix, which represent the potential costs incurred due to overbooking. This involves complex calculations using the binomial probability mass function to estimate scenarios where more passengers show up than seats available, and some passengers are either upgraded to first class or denied boarding.
