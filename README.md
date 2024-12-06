# Project-March-Madness

## Overview
Project March Madness served as a group project conducted to demonstrate learnings from the first year of the Duke Statistical Science Program. See below a description of our project:

With our analysis, we sought to clean and create an effective training and test set based on recent games, then to translate this data into several models. To evaluate our best performing model's validity, we set up several parametric simulations based on historical data and chance, which operated without access to any game play data, flipping a coin to determine the winner of each game. The most intuitive of these simulations, our "blind luck" approach which used a fair coin, was meant to set a lower bound for acceptable performance of any subsequent model. We then proceeded with the "plain vanilla" model, only taking the average win statistics of each ranked position against other ranked positions in the tournament and simulating outcomes. This represented the minimally informed approach, using the seeded positions to simulate an outcome, then determining its average success without any regard for particular features of the incoming teams. Using a large volume of trials, this model gave us percentage chances of wins from each team that would be used to generate an estimated outcome bracket for the recently concluded 2022 iteration of March Madness.

When exploring models, we attempted several approaches:

- Linear Regression
- AdaBoost Regressor with K-Fold Validation
- Ridge Regression with K-Fold Validation
- Random Forest
  - Full data, full feature set
  - Averaged data, full feature set
  - Averaged data, restricted feature set
  - Averaged data, predicting tournament wins
