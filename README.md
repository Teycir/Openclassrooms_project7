# Openclassrooms_project7

Client scoring project. 
The dataset is rebalanced using oversampling, because there are much less non defaulting than defaulting clients. 
We use LightGBM with optimisation and add a surrogate decision tree to enhance the speed of some calculations without losing much precision. 
The surrogate will be used in the API and for the global features importance of the dashboard. 
The API shows list of IDs of clients, does a prediction of solvability, shows importance of features and their description. 

