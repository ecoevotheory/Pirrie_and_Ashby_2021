Source code for the manuscript: Does differential mortality after parental investment affect sex ratio evolution? No.

The following files were created in MATLAB R2020a and tested on 31/08/21:
fig_2.m calculateFitness.m experimentChoice.m symbolicSetupAgeUnions.m symbolicSetupAgeUnionsFrequency.m
modelSolveAgeUnions.c modelSolveAgeUnionsFrequency.c

The code is used to generate figure 2. To run, one must compile the c code in MATLAB as a MEX file, by using:
"mex -setup C; mex modelSolveAgeUnions.c -R2018a" or "mex -setup C; mex modelSolveAgeUnionsFrequency.c -R2018a" respectively. 
Then the figures can be generated by running the script fig_2.m. Model parameters can be changed in the script, 
and one can choose to vary either juvenile or adult mortality, or adult mortality in the exponential model converted to 
frequencies by changing the value of "setupPars.experiment" to either 'uMJAgeUnions', 'uMAAgeUnions', or 
'uMAAgeUnionsFrequency' respectively. 

The following files were created in MATLAB R2020a and tested on 23/08/21:
fig_S1.m sexRatioSweep.m sexRatioSimulation.m sexRatioSweep.mat

This code is used to generate figure S1, using the Gillespie algorithm. To run and generate figure
S1, simply run fig_S1.m (if present, this will use the data file sexRatioSweep.mat).