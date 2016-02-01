One-bit compressive sensing with norm estimation

COPYRIGHT 2014
Karin Knudson <kknudson@math.utexas.edu>, UT Austin
Rayan Saab <rsaab@ucsd.edu>, UCSD
Rachel Ward <ward@math.utexas.edu>, UT Austin

Based on the algorithms described in
K. Knudson, R. Saab, R. Ward, One-bit compressive sensing with norm estimation, 
Preprint, 2014.

------------------------------------


Files included:
    

normEstEDF.m
Matlab function file for estimating the l2 norm of x given binary measurements of the form sign(<a_i, x> - tau),for random Gaussian a, using the empirical distribution function.
See Theorems 10,11, K. Knudson, R. Saab, R. Ward, One-bit compressive sensing with norm estimation, Preprint, 2014.
 
normEstPV.m
Matlab function file for estimating the norm of an N-dimensional signal x given binary measurements y1 of the form sign(a_i x - t_i) (a_i,j ~N(0,1) and t_i~N(0,tau) for nonzero tau) by augmenting x and applying the algorithm from Plan and Vershynin. "One-bit compressed sensing by linear programming." 2013
See Theorem 4, K. Knudson, R. Saab, R. Ward, One-bit compressive sensing with norm estimation, Preprint, 2014.
                
normEstPV_Alternate.m
Matlab function file for estimating the norm of an N-dimensional signal x given binary measurements y1 of the form sign(a_i x - t_i) (a_i,j ~N(0,1) and t_i~N(0,tau) for nonzero tau) by augmenting x and applying the algorithm from Plan and Vershynin. "Robust 1-bit compressive sensing and sparse logistic regression" 2012
See Remark 7, K. Knudson, R. Saab, R. Ward, One-bit compressive sensing with norm estimation, Preprint, 2014.

normRecoveryExample.m
Matlab script to generate an example sparse signal and measurement matrix, and recover the signal’s norm (and the signal itself, if applicable) from one-bit measurements using the methods above.  User should run this file to call the functions normEstEDF, normEstPV and normEstPV_Alternate. 

------------------------------------


Other requirements:

normEstPV.m and normEstPV_Alternate.m make use of the cvx package for convex optimization, (Michael Grant and Stephen Boyd. CVX: Matlab software for disciplined convex programming, version 2.0 beta. http://cvxr.com/cvx, September 2013). CVX is available for download here: http://cvxr.com/cvx/download/.





