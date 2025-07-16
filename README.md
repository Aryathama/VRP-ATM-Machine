# ATM Vehicle Routing Optimization Using Metaheuristics 🚗💨

This project applies and analyzes various metaheuristic algorithms to optimize service routes for BCA Automated Teller Machines (ATMs). The primary objective is to minimize the total travel distance for vehicles while adhering to capacity constraints.

#### Implemented Algorithms: 🧠✨

  * **Enhanced Genetic Algorithm (GA) with 2-Opt Local Search**: A robust implementation of GA with customized operators (like nearest neighbor initialization, order crossover, and 2-opt mutation) and integrated 2-Opt local search for improved route quality.
  * **Simulated Annealing (SA)**: A metaheuristic approach for exploring the solution space by iteratively improving solutions, based on a temperature-dependent probabilistic acceptance criterion.
  * **Ant Colony Optimization (ACO)**: An algorithm inspired by the foraging behavior of ant colonies, utilizing pheromone trails and heuristic information to find optimal paths.
  * **Tabu Search**: A metaheuristic that guides a local search procedure to explore the solution space by maintaining a "tabu list" to avoid cycling and encourage diversification.

#### Key Features: 📊🗺️📈

  * Distance calculations between ATM locations using the Haversine formula.
  * Route visualization using Matplotlib plots and interactive Folium maps (powered by OSRM).
  * Processing of ATM location and demand data from an Excel file (`Dataset VRP ATM BCA.xlsx`).
  * Comparative analysis of the four metaheuristic algorithms, including convergence graphs and result distributions.

#### Dataset: 📂📍

The project utilizes an Excel file, `Dataset VRP ATM BCA.xlsx`. This file contains essential information for each ATM, including its unique ID, Longitude, Latitude, and 'Demand' (service requirements).

#### Dependencies: ⚙️🐍

  * `pandas`
  * `matplotlib`
  * `scikit-learn`
  * `seaborn`
  * `numpy`
  * `folium`
  * `requests`
  * `polyline`
