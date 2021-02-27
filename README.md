# Option-Pricing 


<img src="img/sim_path_1000.png" width="2000"> 


- <img src="img/python.png" width="20"> *Numpy/Pandas*

- Formulations mathématiques et projet complet disponible en pdf.

## Modèle de Black & Scholes et méthode de Monte Carlo 
  - <img src="img/python.png" width="20"> Class BS : Formule fermée de Black & Scholes et les principales greeks associées
  - <img src="img/python.png" width="20"> Class MonteCarloBS (parente) | Class MonteCarloEuropeanApplication : Monte-Carlo pour Call & Put 
  - <img src="img/python.png" width="20"> Class MonteCarloBS_Basket : Application Monte-Carlo pour un panier d'actifs
  
## Pricing d'options asiatiques et réduction de variance
  - <img src="img/python.png" width="20"> Class MonteCarloBSPathDependant : dates en fractions numérique ou de type TimeStamp pandas pour pricing (précision seconde) 
  - <img src="img/python.png" width="20"> Class MonteCarloBS_Asian
    - exemple output : <img src="img/ex_output.png" width="2000">
  - Réduction de variance par variables antithétiques et de contrôle
    
## Pricing Options à barrières Up&In, Down&Out
- <img src="img/python.png" width="20"> Class MonteCarloBS_UpAndOut | Class MonteCarloBS_DownAndIn
- Réduction de variance par Monte Carlo Conditionnel

## EDP pour Black & Scholes
- Résolution de l'équation de Black & Scholes par EDP

## EDS pour Black & Scholes et modèle de Heston
- <img src="img/python.png" width="20"> Class EDS | Class EDS_BS : approximation de la solution de BS par schéma d'Euler et de Milstein
- <img src="img/python.png" width="20"> Class Heston : modèle de Heston pour volatilité stochastique, dérivant des classes MonteCarloBS et EDS.
  - Smile de volatilité
  - Evolution du smile en fonction des paramètres

