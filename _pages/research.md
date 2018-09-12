---
layout: archive
title: "Research"
permalink: /research/
use_math: true
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
      
4. **Multiple Instance Learning (MIL) in Breast Cancer Histology Images** (Feb '18 - Present) <br/>
    **Guide : Prof. Amit Sethi, EE Department, IIT Bombay** <br/>
    * **MIL** is an **unsupervised learning problem** where the label of the entire image (“bag”) is given and the labels
      of the patches (“instances”) in the image are to be determined from this. <br/>
    * Currently working on **self-supervised learning** using the proxy tasks of **colorization** and **novel gradient based
      segmentation** (work in progress!), to learn good **embeddings** which can be used for **deep attention based MIL**. <br/>
    * Tried **Bayesian Learning** for MIL using features extracted from **auto-encoders** and obtained **results comparable to state of
      the art** for the **Bisque data set**. However, this method did not generalize well! **CODE & REPORT!!!** <br/>
      
5. **Sentence Compression Using Deep Learning** (Mar '18 - May '18) <br/>
    **Guide :  Prof. Sunita Sarawagi, CSE Department, IIT Bombay** <br/>
    * Designed a **bi-directional 3-layer LSTM** model for **sentence compression** by modelling it as a binary classification
      problem (which words to retain/delete). Compared it with the method proposed in “**Sentence
      Compression by Deletion with LSTMs**” by **Google NLP Research** and got **marginally better results**. <br/>
    * The detailed method and results can be found [here](https://github.com/rudrajit15/Sentence-Summarization-using-LSTMs/blob/master/Report/AML%20Report.pdf). The code can be found [here](https://github.com/rudrajit15/Sentence-Summarization-using-LSTMs/tree/master/Codes).<br/>
    
6. **Speeding up Kernel PCA (KPCA)** (July '17 - Oct '17) <br/>
    **Guide : Prof. Suyash Awate, CSE Department, IIT Bombay** <br/>
    * Used the **improved Nyström method** to obtain a **low rank** approximation to the Gram matrix. Using this,
      developed a **fast algorithm for eigenvector computation** in KPCA, **improving time complexity** from $O(n^{2}p)$
      to $O(np^{2})$, where n is the number of data points and p << n is the rank of the approximated Gram matrix. <br/>
    * Simulated the above algorithm and obtained almost a **linear speed up** over MATLAB’s “eigs” function with
      **negligible error** in the obtained eigenvectors and eigenvalues. **CODE & REPORT!!!** <br/>
     
   
    
