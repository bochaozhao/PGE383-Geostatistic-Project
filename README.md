# PGE383-Geostatistic-Project
project files for PGE383 Geostatistics taught by Michael J. Pyrcz at University of Texas at Austin (https://github.com/GeostatsGuy)

Dependencies:
This project utilizes GeostatsPy package. The GeostatsPy Package brings GSLIB: Geostatistical Library (Deutsch and Journel, 1998) functions to Python. GSLIB is extremely robust and practical code for building spatial modeling workflows. The repository for GeostatsPy package can be found here: https://github.com/GeostatsGuy/GeostatsPy


The updates are organized as follows:

# Update 2 
The purpose of this update is to subject the data to further evaluation, by understanding its spatial distribution, identifying and correcting for sampling bias, then performing subsequent analysis on it. 
The work included:
1. Applying cell declustering technique to correct sampling bias in the data
2. Statistical hypothesis testing for porosity and permeability values for each facies
3. Heterogeneity assessment of porosity and permeability values using multiple metrics 
4. Preliminary uncertainty model for porosity and permeability based on facies
5. An initial estimate of oil in place (in barrels)

# Update 3 
The purpose of this update is to develop a preliminary understanding of the spatial continuity of facies, porosity, and permeability across the area of interest based on variogram modeling.
The work included:
1. Generating variogram maps for porosity (all facies) using declustered data
2. Calculating isotropic and directional variograms for facies, porosity, and permeability
3. Assessing heterogeneity and analyzing spatial continuity by modeling semivariograms

# Update 4
The purpose of this update is to apply spatial estimation analysis to assess the spatial uncertainties over our study area, given the available data and the models of spatial continuity previously built. 
The work included:
1. Calculating the probability of each facies across the reservoir
2. Computing the Kriging estimate and variance for porosity and permeability over the entire prospect, for each facies
3. Building a combined model (cookie cutter approach) with porosity and permeability for the most likely facies at all locations
4. Calculating the values for porosity and permeability of most likely facies and reporting the local  P10 and P90 map
5. Picking two candidate well locations and providing a pre-drill porosity uncertainty distribution accounting for the probability of each facies

# Update 5
The purpose of this update is to build a suite of simulated realizations to represent subsurface uncertainty. 
The work included:
1. Simulate 20 realizations of facies.
2. Simulate 20 realizations of porosity by-facies. Use trend model with
trend and residual workflow.
3. Cosimulate 20 realizations of permeability by facies.
4. Check the input statistics (histograms and variograms). For gam
calculations find an angle in cell offsets closest to major and minor.
5. Combine the porosity and permeability by-facies with the cookie
cutter approach.

# Update 6
The purpose of this update is to build a suite of scenarios and realizations to represent subsurface uncertainty. 
The work included:
1. Calculation of the uncertainty in facies proportions and average porosity by using the spatial bootstrap method
2. Propagation of uncertainty in facies proportions and porosity average to porosity realizations
3. Integration of the local uncertainty into the calculation of oil in place
