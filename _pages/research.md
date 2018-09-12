---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
1.  **Improving Optimization in Deep Learning - Master’s Thesis** (June '18 - Present) <br/>
    **Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay** <br/>
    * As of now, proposed a **novel randomized iterative** algorithm to detect whether a critical point (i.e. a point where the
    derivatives of the loss function with respect to the parameters are zero) is a local minima or a **saddle point**
    and to escape that point if it is a **saddle point**, without requiring to compute the **Hessian**. <br/>
    * Derived an **upper bound** on the **expected number of iterations**, which is **logarithmic** with respect to the
    number of positive eigenvalues of the Hessian at that point and **faster than linearithmic** with respect to
    the inverse of the magnitude of the minimum eigenvalue of the Hessian. The **complexity wrt the minimum
    eigenvalue** of the Hessian is **better** than that of existing algorithms. <br/>
    * Also, in relation to the complexity of the proposed algorithm, obtained approximate **upper and lower bounds**
    for the **expected number of negative eigenvalues** of the Hessian (known as the index) at a point, as a function
    of the loss value at that point, for a single hidden layer neural network with the **cross-entropy loss function**.
    This is the **first attempt** at index computation for the cross-entropy loss function. <br/>
    * Paper submitted to **AAAI-19**. <br/>
    
 2. **Sparse Kernel PCA (SKPCA) for Outlier Detection** (Nov '17 - May '18) <br/>
    **Guide : Prof. Suyash Awate, CSE Department, IIT Bombay** <br/>
    * Proposed a **novel SKPCA** algorithm by formulating it as a **constrained optimization problem** with **elastic
      net regularization** in the kernel space. Tested it on **5 real world datasets** and showed that it **outperforms**
      the most recent SKPCA method with **lesser parameter tuning**. <br/>
    * Also presented a **new probabilistic proof** to justify the **existence of sparse solutions** in KPCA using the
      RBF kernel, which is the **first attempt** in this direction. <br/>
    * **Paper accepted** for **oral presentation** in **IEEE ICMLA 2018**. <br/>
    
 3. **Non-linear blind compressed sensing** (June '18 - Present) <br/>
    **Guide : Prof. Ajit Rajwade, CSE Department, IIT Bombay** <br/>
    * Working on **blind compressed sensing** (jointly estimating the sparse basis & sparse codes) under **non-linear
      transformations** of data to make the noise model **Gaussian**, such as the **Anscombe transform** for **Poisson
      measurements????**. This has not been done before and is **challenging** due to the **non-linearity** and the highly
      **non-convex nature** of the problem. <br/>
    * Using Stochastic Gradient Descent (**SGD**) to solve the **non-linear least squares** problem with **L1** penalty
      (**Lasso**) imposed for sparsity. **BOUND!!!** <br/>
    
