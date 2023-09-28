# Pricing_Exotic_Options_using_Monte_Carlo_Simulation
Although there are many complex exotic options, in this code, the examples of Asian and Lookback options have been taken. A brief description of the option structure and payoff is given. With both these being path dependent options, the entire price path the underlying takes needs to be captured and used in the payoff, as opposed to Vanilla options, whose price at expiry is only what matters (european)
There are a couple fo ways in which exotic options can be priced, Monte Carlo simulation and finite difference methods. Monte Carlo simulation has been used in this case. The price path, which is continuous has been dicretized using the Euler method and the time steps have been set equal to a day.
## Monte Carlo Simulation:
Monte Carlo simulation generates, many (100000 in this instance) outcomes using a random number generator. The price paths that are generated have been stored in a dataframe. This dataframe is used as an input to value the options.
## Options: 
The options have been structured as objects to call out the various versions of the options. These options are then called using the input values(specified in the file) and the dataframe generated from the Monte Carlo Simulation to value them. In this instance, the Call Rate Options for both Asian and Lookback options have been used for comparison. The vanilla option values have also been included for a better understanding of the payoffs.
## Varying the input values:
The input values are varied in-turn and the impact of that is seen on the price of the options. The payoffs are plotted for the three options for each input value being varied to understand the movement of the payoffs.
