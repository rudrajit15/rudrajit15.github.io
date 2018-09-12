
---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

1.  **Improving Optimization in Deep Learning - Master’s Thesis** (June '18 - Present) <br/>
    **Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay** <br/>
    * As of now, proposed a novel randomized iterative algorithm to detect whether a critical point (i.e. a point where the
    derivatives of the loss function with respect to the parameters are zero) is a local minima or a saddle point
    and to escape that point if it is a saddle point, without requiring to compute the Hessian. <br/>
    * Derived an upper bound on the expected number of iterations, which is logarithmic with respect to the
    number of positive eigenvalues of the Hessian at that point and faster than linearithmic with respect to
    the inverse of the magnitude of the minimum eigenvalue of the Hessian. The complexity wrt the minimum
    eigenvalue of the Hessian is better than that of existing algorithms. <br/>
    * Also, in relation to the complexity of the proposed algorithm, obtained approximate upper and lower bounds
    for the expected number of negative eigenvalues of the Hessian (known as the index) at a point, as a function
    of the loss value at that point, for a single hidden layer neural network with the cross-entropy loss function.
    This is the first attempt at index computation for the cross-entropy loss function. <br/>
    * Paper submitted to AAAI-19. <br/>
