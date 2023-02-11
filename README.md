**Pacmann AI**

# sampling: Non-adaptive and adaptive sampling based on residuals for PINN

[@github:zulkarnainprastyo](https://github.com/zulkarnainprastyo), [@medium:Zulkarnain Prastyo](https://medium.com/@zulkarnain.prastyoumb23093)

## Table of Contents

* [Introduction & Background](#introduction-&-background)
* [Sampling Design](#sampling-design)
* [Analysis](#analysis)
* [Conclusion](#conclusion)
* [References](#references)
* [Citation](#citation)


## Introduction & Background
- Explain the problem & why it's important to solve.
- We want to create something scientific & data-driven.
- Explain the background of the problem with supporting data.
- Explain the benefits of your research results.

In recent years, physics-informed neural networks (PINNs) [1] have emerged as a powerful tool for solving forward and inverse problems of partial differential equations (PDEs) using deep neural networks (DNNs) [2, 3, 4].
The effect of residual points on PINNs is intuitively similar to the effect of mesh points on FEM, and thus the location and distribution of these residual points should be critical to the performance of PINNs.
In this study, I looked at
 Extensively compared the performance of different uniform sampling methods, including (1) equispaced uniform grid, (2) uniformly random sampling, (3) LHS, (4) Sobol sequence, (5) Halton sequence, and (6) Hammersley sequence.
In this study, I considered a total of 10 different sampling techniques, including seven non-adaptive sampling techniques (six different uniform sampling and one uniform sampling with resampling) and three adaptive sampling methods (RAR, RAD, and RAR-D).

 I compared the performance of these sampling methods on four PDE forward problems and examined the effect of the number of residual points.

## Sampling Design
- Describe it according to the stages described on the previous page.
- Create illustrations to taste.
- Create math equations neatly. For example, using Latex.
- Also explain the reasons why you chose the design.

PINNs use uniform sampling and nonuniform residual-based adaptive sampling to improve accuracy and training efficiency.

## Analysis
- Describe the results of your sampling design.
- Does the result make sense?
- What is the effectiveness of your sampling design? For example from the side:
 -Cost
 -Time
 - Resources needed
- Explain the weaknesses/problems/limitations that should be known from your sampling design and how to overcome them.

## Conclusion
- Show the conclusions of the sampling design & the results you made.
- again
    - Sampling design results
    - Design excellence
    - design flaws


## References
[1] Raissi, M., Perdikaris, P., & Karniadakis, G. E. (2019). Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations. Journal of Computational physics, 378, 686–707.
[2] Raissi, M., Yazdani, A., & Karniadakis, G. E. (2020). Hidden fluid mechanics: Learning velocity and pressure fields from flow visualizations. Science, 367(6481), 1026–1030.
[3] Lu, L., Meng, X., Mao, Z., & Karniadakis, G. E. (2021). DeepXDE: A deep learning library for solving differential equations. SIAM review, 63(1), 208–228.
[4] Karniadakis, G. E., Kevrekidis, I. G., Lu, L., Perdikaris, P., Wang, S., & Yang, L. (2021). Physics-informed machine learning. Nature Reviews Physics, 3(6), 422–440.
[5] Chen, Y., Lu, L., Karniadakis, G. E., & Dal Negro, L. (2020). Physics-informed neural networks for inverse problems in nano-optics and metamaterials. Optics express, 28(8), 11618–11633.
[6] Yazdani, A., Lu, L., Raissi, M., & Karniadakis, G. E. (2020). Systems biology informed deep learning for inferring parameters and hidden dynamics. PLoS computational biology, 16(11), e1007575.
[7] Daneker, M., Zhang, Z., Karniadakis, G. E., & Lu, L. (2022). Systems Biology: Identifiability analysis and parameter identification via systems-biology informed neural networks. arXiv preprint arXiv:2202.01723.
[8] Lu, L., Pestourie, R., Yao, W., Wang, Z., Verdugo, F., & Johnson, S. G. (2021). Physics-informed neural networks with hard constraints for inverse design. SIAM Journal on Scientific Computing, 43(6), B1105-B1132.
[9] Pang, G., Lu, L., & Karniadakis, G. E. (2019). fPINNs: Fractional physics-informed neural networks. SIAM Journal on Scientific Computing, 41(4), A2603-A2626.
[10] Zhang, D., Lu, L., Guo, L., & Karniadakis, G. E. (2019). Quantifying total uncertainty in physics-informed neural networks for solving forward and inverse stochastic problems. Journal of Computational Physics, 397, 108850.
[11] Psaros, A. F., Kawaguchi, K., & Karniadakis, G. E. (2022). Meta-learning PINN loss functions. Journal of Computational Physics, 458, 111121.
[12] Yu, J., Lu, L., Meng, X., & Karniadakis, G. E. (2022). Gradient-enhanced physics-informed neural networks for forward and inverse PDE problems. Computer Methods in Applied Mechanics and Engineering, 393, 114823.
[13] Wang, S., Teng, Y., & Perdikaris, P. (2021). Understanding and mitigating gradient flow pathologies in physics-informed neural networks. SIAM Journal on Scientific Computing, 43(5), A3055-A3081.
[14] Xiang, Z., Peng, W., Liu, X., & Yao, W. (2022). Self-adaptive loss balanced Physics-informed neural networks. Neurocomputing, 496, 11–34.
[15] Gu, Y., Yang, H., & Zhou, C. (2021). Selectnet: Self-paced learning for high-dimensional partial differential equations. Journal of Computational Physics, 441, 110444.
[16] Li, W., Zhang, C., Wang, C., Guan, H., & Tao, D. (2022). Revisiting PINNs: Generative adversarial physics-informed neural networks and point-weighting method. arXiv preprint arXiv:2205.08754.
[17] Meng, X., Li, Z., Zhang, D., & Karniadakis, G. E. (2020). PPINN: Parareal physics-informed neural network for time-dependent PDEs. Computer Methods in Applied Mechanics and Engineering, 370, 113250.
[18] Jagtap, A. D., & Karniadakis, G. E. (2021, March). Extended Physics-informed Neural Networks (XPINNs): A Generalized Space-Time Domain Decomposition based Deep Learning Framework for Nonlinear Partial Differential Equations. In AAAI Spring Symposium: MLPS (pp. 2002–2041).
[19] Wight, C. L., & Zhao, J. (2020). Solving allen-cahn and cahn-hilliard equations using the adaptive physics informed neural networks. arXiv preprint arXiv:2007.04542.
[20] Mattey, R., & Ghosh, S. (2022). A novel sequential method to train physics informed neural networks for Allen Cahn and Cahn Hilliard equations. Computer Methods in Applied Mechanics and Engineering, 390, 114474.
[21] Haitsiukevich, K., & Ilin, A. (2022). Improved training of physics-informed neural networks with model ensembles. arXiv preprint arXiv:2204.05108.
[22] Lagari, P. L., Tsoukalas, L. H., Safarkhani, S., & Lagaris, I. E. (2020). Systematic construction of neural forms for solving partial differential equations inside rectangular domains, subject to initial, boundary and interface conditions. International Journal on Artificial Intelligence Tools, 29(05), 2050009.
[23] Dong, S., & Ni, N. (2021). A method for representing periodic functions and enforcing exactly periodic boundary conditions with deep neural networks. Journal of Computational Physics, 435, 110242.
[24] Halton, J. H. (1960). On the efficiency of certain quasi-random sequences of points in evaluating multi-dimensional integrals. Numerische Mathematik, 2, 84–90.
[25] Binder, K. (1986). Introduction: Theory and "technical" aspects of Monte Carlo simulations. Monte Carlo methods in statistical physics, 1–45.
[26] Dong, S., & Ni, N. (2021). A method for representing periodic functions and enforcing exactly periodic boundary conditions with deep neural networks. Journal of Computational Physics, 435, 110242.
[27] Nabian, M. A., Gladstone, R. J., & Meidani, H. (2021). Efficient training of physics‐informed neural networks via importance sampling. Computer‐Aided Civil and Infrastructure Engineering, 36(8), 962–977.

## Citation

Please cite this article as follows, or use the medium entry below.
