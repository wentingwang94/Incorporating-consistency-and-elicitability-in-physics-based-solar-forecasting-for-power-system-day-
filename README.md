# Physics-based-solar-forecasting-for-power-system-day-ahead-dispatching


### Requirments：
The code is written in Python, and some packages should be installed before the scripts can be executed smoothly.  
  * Package [pandas](https://pandas.pydata.org/pandas-docs/stable/index.html) is a fast, BSD-licensed library that provides high-performance data structures and data analysis tools.
  * Package [numpy](https://numpy.org/doc/stable/) is the fundamental package for scientific computing.
  * Package [pvlib](https://pvlib-python.readthedocs.io/en/stable/) provides functions for simulating the performance of PV systems.
  * Package [scipy](https://scipy.org/) provides algorithms for scientific computing.
  * Package [sklearn](https://scikit-learn.org/stable/) is the basic package for machine learning.
  * Package [gurobipy](https://pypi.org/project/gurobipy/) is a mathematical optimization software library.

Other Python packages that used for plotting the results include [plotnine](https://plotnine.readthedocs.io/en/stable/) and [matplotlib](https://matplotlib.org/). 

### Data: 
A total of 5 [XXX_ENS.csv], [McClear_UPV.csv](https://github.com/wentingwang94/Physics-based-solar-forecasting-for-power-system-day-ahead-dispatching/blob/main/data/McClear_UPV.csv), [ENS_UPV.csv](https://github.com/wentingwang94/Physics-based-solar-forecasting-for-power-system-day-ahead-dispatching/blob/main/data/ENS_UPV.csv), [HRES_UPV.csv], [electric_load](https://github.com/wentingwang94/Physics-based-solar-forecasting-for-power-system-day-ahead-dispatching/blob/main/data/electric_load.csv), and [simulated_UPV.csv] files are provided. These files contain four years (2017--2020) of the ECMWF ENS forecast data for five stations (xxx denotes the three-letter station abbreviations), four years (2017--2020) of the ECMWF ENS forecasting data for the project-level PV plant, clear-sky irradiance for the project-level PV plant, ECMWF HRES forecast data, electric load, and simulated PV power output of the project-level PV plant.

### Code: 
A total of four Python scripts, namely, [beta_med.py], [proposed_method.py], [benchmark_method.py], and [dispatch_model.py] are provided for reproducibility. The file names are self-explanatory. In that, [beta_med.py] provides the the computation of $\beta$-median; [physics-based_forecasting_method.py] provides the two-step physics-based solar power forecasting method; [benchmark_forecasting_method.py] reproduces the benchmark using gradient boosting; and [dispatch_model] reproduces the day-ahead power system dispatch results. 
