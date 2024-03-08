# Approximate-Bayesian-Computation-for-Inferring-Waddington-Landscapes-from-Single-Cell-Data

This is the code reproduce the result of ABC-SMC for single cell data inference with different distance metrics.
"mmd.ipynb" contains the code for reproducing the result of ABC-SMC with MMD as distance metric. Results for other distance metric 
can be obtained by modifying the the set up of ABC-SMC algorithm with distance metric by modifying the "simdist" function to desired distance metric.
The running time would be around 3-4 days for MMD/Optimal Transprot, 7-10 days for Bhattacharyya distance on a 50 CPUs cluster.

".csv" files contains the result of ABC-SMC for different distance metrics. In each file, there are 1000 particles for each set of parameters which are obtained 
from ABC-SMC with different distance metrics.

".jld2" files contains the result of ABC-SMC for different distance metrics as above. One can draw weighted particles from each file to simulate the results.  

"output_analysis.ipynb" contains the code for sensitivity analysis of parameters(PCA based approach) and performance test with log
transformed probability of cells in pluripotent states as metrics for results obtained from each distance metric. 

"pair_plot.ipynb" generate the pair wise density plot for the ABC-SMC result.
