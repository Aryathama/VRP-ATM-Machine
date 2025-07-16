### ATM Vehicle Routing Optimization Using Metaheuristics

This project applies and analyzes various metaheuristic algorithms to optimize service routes for BCA Automated Teller Machines (ATMs). The primary objective is to minimize the total travel distance for vehicles while adhering to capacity constraints.

#### Implemented Algorithms:

  * **Enhanced Genetic Algorithm (GA) with 2-Opt Local Search**: A robust genetic algorithm tailored for VRP, incorporating specialized operators (like nearest neighbor initialization, order crossover, and 2-opt mutation) and integrated 2-Opt local search for improved route quality.
  * **Simulated Annealing (SA)**: A metaheuristic approach for exploring the solution space by iteratively improving solutions, based on a temperature-dependent probabilistic acceptance criterion.
  * **Ant Colony Optimization (ACO)**: An algorithm inspired by the foraging behavior of ant colonies, utilizing pheromone trails and heuristic information to find optimal paths.
  * **Tabu Search**: A metaheuristic that guides a local search procedure to explore the solution space by maintaining a "tabu list" to avoid cycling and encourage diversification.

#### Key Features:

  * Distance calculations between ATM locations using the Haversine formula.
  * Route visualization using Matplotlib plots and interactive Folium maps, with realistic routing powered by the Open Source Routing Machine (OSRM) API.
  * Data processing for ATM location and demand data from an Excel file (`Dataset VRP ATM BCA.xlsx`).
  * Comparative analysis of the four metaheuristic algorithms, including convergence graphs showing best distance over iterations and box plots showing result distributions over multiple runs.

#### Dataset:

The project utilizes an Excel file, `Dataset VRP ATM BCA.xlsx`, which is converted to CSV format. This file contains essential information for each ATM, including its unique ID, Longitude, Latitude, and 'Demand' (service requirements).

#### Results:

The analysis demonstrates the effectiveness of these metaheuristics in solving VRP instances. For the given dataset (50 customers, vehicle capacity 80):

  * **Enhanced GA + 2-Opt**: Achieved a best total distance of **69.45 km** across 6 optimized routes.
  * **Simulated Annealing**: Achieved a best total distance of **74.63 km** across 6 routes.
  * Performance for **ACO** and **Tabu Search** is also analyzed and compared within the notebook, showcasing their results and convergence characteristics.

#### Dependencies:

  * `pandas`
  * `matplotlib`
  * `scikit-learn`
  * `seaborn`
  * `numpy`
  * `folium`
  * `requests`
  * `polyline`
