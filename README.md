EDGE-Roaches
============
Files:

ROACHode.m This file contains the system of ODES, and sets most of the parameter values.

Treatment.m This file creates the treatment function. 

TreatmentRoachsolver.m runs the solver for the system of ODES and a given treatment plan.


TreatmentRun.m can be used to run a sinlge simulation. It takes a vector of {0,1,2} as the input which represents the treatment plan. The length of the lector corresponds to the number of days of treatment. The values {0,1,2} represent the amount of pesticide to apply each day. Example: In the command window type
>> TreatmentPlan=1*ones(1,120); %%  same low does treatment everyday
>> TreatmentRun(TreatmentPlan); 


GeneticAlgorithm.m can be used to find an optimal treatment plan. It randomly creates treatment plan (vectors containing {0,1,2}), and runs a genetic algorithms to find the optimal treatment plan. The number of treatment plans in each "generation", and the number of generations (maxgens) can be specified in the code. 
