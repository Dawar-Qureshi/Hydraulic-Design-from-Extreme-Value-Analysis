# Hydraulic Design from Extreme Value Analysis

### Bayesian GEV-based Extreme Value Analysis applied to stormwater and hydraulic design.



## Overview

This project explores how probabilistic rainfall modeling can support practical hydraulic design. Using the Generalized Extreme Value (GEV) distribution and Bayesian inference, I estimated rainfall return levels for different design periods (such as 10-, 50-, and 100-year events).  The goal is to show how uncertainty in extreme rainfall can be quantified and integrated into the design of **stormwater drainage systems** and other hydraulic structures.  This approach provides a more resilient and data-driven alternative to traditional deterministic design methods.



## Methodology

1. **Data Preparation**
   - Historical rainfall data was collected and processed to extract annual maximum rainfall (AMR) values.
   - The data was checked for trends, missing values, and consistency.

2. **Extreme Value Modeling**
   - The AMR series was fitted to a GEV distribution.
   - Bayesian inference was performed using **PyMC** to estimate the GEV parameters:
     - Location (μ)
     - Scale (σ)
     - Shape (ξ)

3. **Return Level Estimation**
   - Posterior samples were used to calculate rainfall return levels with credible intervals.
   - Results include rainfall estimates for 10-, 25-, 50-, and 100-year events.

4. **Hydraulic Design Application**
   - The estimated rainfall intensities were applied to the design of stormwater pipes.
   - The workflow demonstrates how probabilistic rainfall analysis can guide hydraulic design under uncertainty.



## Tools and Libraries

- **Python 3.11**
- **PyMC** – Bayesian inference  
- **NumPy**, **Pandas** – data handling  
- **Matplotlib**, **ArviZ** – visualization and uncertainty plots  
- **SciPy** – statistical analysis  
- **Jupyter Notebook** – workflow and documentation  



## Example Outputs

- Posterior distributions of GEV parameters  
- Rainfall return level curves with 95% credible intervals  
- Design rainfall intensities for different return periods  
- Example pipe sizing calculations using the probabilistic rainfall data




## Applications

- Stormwater and sewer system design  
- Culvert and open channel design  
- Flood risk assessment  
- Climate resilience and uncertainty analysis in hydrology  



## References

- Coles, S. (2001). *An Introduction to Statistical Modeling of Extreme Values.* Springer.  
- Beven, K. (2012). *Rainfall–Runoff Modelling: The Primer.* Wiley.  
- PyMC Documentation: [https://www.pymc.io](https://www.pymc.io)



## Author

**Dawar Qureshi**  
M.Sc. Hydro Science and Engineering  
Research interests: Design & operation of hydraulic infrastructure, Flood risk modelling, CFD applications in hydraulic engineering.   



## License

This project is licensed under the **MIT License** — free to use and modify with attribution.

