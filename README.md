GAUSSIAN COPULA:
CDO pricing model following homogeneous Gaussian copula logic and Gauss-Hermite integration. Separates the payment legs into three parts: Expected Tranche Principal, Expected Regular Spread Payments, Expected Accrual Payments. 
Given an upfront, spread, and lower and upper tranche bounds, the model can find the compound correlations and base correlations for tranches.
The model can also find upfront and spread for a given compound correlation and lower and upper tranche bounds.
Portfolio size, recovery rate, and integration points for Gauss-Hermite can all be modified when initializing the class.
NB: Hardcoded for CDS maturities!  

t-COPULA:
Expansion of the Gaussian Copula, where the systematic and idiosyncratic factors are instead t-distributed with v degrees of freedom.
This necessitates the use of characteristic functions and adaptive quadrature to integrate over the systematic factors.
Possesses the same capabilities as the Gaussian Copula, only the underlying assumption is altered and the engine to generate results
NB: Hardcoded for CDS maturities!  
