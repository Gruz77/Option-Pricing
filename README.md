# Option-Pricing 


<img src="img/sim_path_1000.png" width="2000"> 


- <img src="img/python.png" width="20"> *Numpy/Pandas*

- Mathematical formulations and full project available in pdf.

## Black & Scholes and Monte Carlo methods
  - <img src="img/python.png" width="20"> Class BS : Black & Scholes closed formula and the main associated greeks
  - <img src="img/python.png" width="20"> Class MonteCarloBS (parent) | Class MonteCarloEuropeanApplication : Monte Carlo for Call & Put 
  - <img src="img/python.png" width="20"> Class MonteCarloBS_Basket : Monte-Carlo application for a basket of assets
  
## Asian options pricing and variance reduction
  - <img src="img/python.png" width="20"> Class MonteCarloBSPathDependant: dates in numeric fractions or TimeStamp pandas for pricing (precision : seconds) 
  - <img src="img/python.png" width="20"> Class MonteCarloBS_Asian
    - exemple output : <img src="img/ex_output.png" width="2000">
  - Variance reduction by antithetical and control variables
    
## Pricing Options with Up&In, Down&Out barriers
- <img src="img/python.png" width="20"> Class MonteCarloBS_UpAndOut | Class MonteCarloBS_DownAndIn
- Variance Reduction by Conditional Monte Carlo

## PDE for Black & Scholes
- Solving the Black & Scholes equation using PDE

## EDS for Black & Scholes and Heston model
- <img src="img/python.png" width="20"> Class EDS | Class EDS_BS : approximation of the BS solution by Euler and Milstein scheme
- <img src="img/python.png" width="20"> Class Heston: Heston model for stochastic volatility, deriving from MonteCarloBS and EDS classes.
  - Volatility Smile
  - Evolution of the smile as a function of the parameters

