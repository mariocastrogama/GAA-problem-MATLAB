# GAA-problem-MATLAB
This is a conversion of the General Aviation Aircraft problem into MATLAB

General Aviation Aircraft Problem using Response Surface Model
 
Original development was made at the Pennsylvania State University by
Dr. Timothy Simpson, Dr. Patrick Reed, Brayan D'Souza, Ruchit Shah,
Matthew Woodruff, and David Hadka.  

Adaptation to MATLAB was performed by Mario Castro-Gama

If this software is used in
academic publications, please cite the following papers accordingly:

    [1] Simpson, T.W., Chen, W., Allen, J.K., and Mistree, F. (1996),
      "Conceptual design of a family of products through the use of
       the robust concept exploration method," in 6th AIAA/USAF/NASA/
       ISSMO Symposium on Multidiciplinary Analysis and Optimization,
       vol. 2, pp. 1535-1545.
 
   [2] Simpson, T.W., D'Souza, B.S. (2004), "Assessing variable levels
       of platform commonality within a product family using a
       multiobjective genetic algorithm," Concurrent Engineering:
       Research and Applications, vol. 12, no. 2, pp. 119-130.
 
   [3] Shah, R., Reed, P.M., and Simpson, T.W. (2011), "Many-objective
       evolutionary optimization and visual analytics for product
       family design," Multiobjective Evolutionary Optimisation for
        Product Design and Manufacturing, Springer, London, pp. 137-159.
   
   [4] Woodruff, M.J., Reed, P.M. and Simpson, T.W. (2013), "Many objective 
       visual analytics: rethinking the design of complex engineered systems 
       Struct Multidisc Optim, 48, 201–219

/* Implementation follows [3] and [4] */

 Input variables
   var: the array of decision variables (27)

 Output variables
   obj: the array of objectives (10)
   con: the array of constraints (1)

  Developed in MATLAB by:
  Mario Castro Gama
  PhD Researcher
  2016-08-01

  

The number of decision variables
 GAA_Number_variables = 27;

The number of objectives
 GAA_Number_objectives = 10;

The number of constraints
 GAA_Number_constraints = 1;

The decision variable lower bounds
 GAA_Bounds_lower = [ 0.240, 7.000, 0.000, 5.500, 19.000, 85.000, 14.000, 3.000, 0.460, ...
                       0.240, 7.000, 0.000, 5.500, 19.000, 85.000, 14.000, 3.000, 0.460, ...
                       0.240, 7.000, 0.000, 5.500, 19.000, 85.000, 14.000, 3.000, 0.460];
The decision variable upper bounds
  GAA_Bounds_upper = [ 0.480, 11.000, 6.000, 5.968, 25.000, 110.000, 20.000, 3.750, 1.000, ...
                       0.480, 11.000, 6.000, 5.968, 25.000, 110.000, 20.000, 3.750, 1.000, ...
                       0.480, 11.000, 6.000, 5.968, 25.000, 110.000, 20.000, 3.750, 1.000];
