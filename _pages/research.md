---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
use_math: true
---
**Research Experience:**
1. **On the Separability of Classes with the Cross-Entropy Loss Function** (Jan '19 - May '19) <br/>
    *Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay* <br/>
    * Analysis of the **separability of classes** attained with the **cross-entropy loss** function for classification problems by theoretically analyzing the **intra-class distance** and **inter-class distance** (i.e. the distance between any two points belonging to the same class and different classes, respectively) in the feature space, i.e. the space of representations learned by neural networks. <br/>
    * Specifically, considered an arbitrary network architecture having a fully connected final layer with Softmax activation and trained using the cross-entropy loss. Derived expressions for the value and the distribution of the squared L2 norm of the product of a network dependent matrix and a random intra-class and inter-class distance vector (i.e. the vector between any two points belonging to the same class and different classes), respectively, in the learned feature space (or the transformation of the original data) just before Softmax activation, as a function of the cross-entropy loss value. <br/>
    * Main result of the analysis is the derivation of a **lower bound for the probability with which the inter-class distance is more than the intra-class distance** in this feature space, as a function of the loss value. As per intuition, the probability with which the inter-class distance is more than the intra-class distance decreases as the loss value increases, i.e. **the classes are better separated when the loss value is low**. <br/>
    * First work of theoretical nature trying to explain the separability of classes in the feature space learned by neural networks trained with the cross-entropy loss function. Paper submitted to **NeurIPS 2019**. <br/>
    
 2. **Extremal Eigenvalue Analysis of the Hessian and a Learning Rate Choice for Stochastic Gradient Descent** (Jan '19 - June '19) <br/>
    *Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay* <br/>
    * Analysis of the **extremal (maximum and minimum) eigenvalues of the Hessian** matrix is of significance, especially for setting the learning rate/step-size in gradient based optimization algorithms and to gain insight about the performance of saddle point escaping algorithms. <br/>
    * In relation to this, presented a technique to obtain **probabilistic bounds for the extremal eigenvalues of the Hessian** at a point, as a function of the loss value at that point. The technique is based on **matrix concentration inequalities** and the computations are performed for a single hidden layer neural network with the cross-entropy loss function. In theory, the technique can be extended to more complicated architectures and loss functions, provided the Hessian obeys a certain structure. <br/>
    * Secondly, proposed a method to **automatically set the learning rate in mini-batch stochastic gradient descent**, a core part
of which, also relies on matrix concentration inequalities. Two schemes have been proposed - one in which the **batch size is kept fixed** and another one in which the **batch size is increased with the number of epochs** allowing us to choose much higher learning rates than those in the first scheme, potentially leading to **faster training**. <br/>
    * Paper submitted to **SIAM Journal on Mathematics of Data Science (SIMODS)**. <br/>
    
3.  **A Randomized Algorithm to Detect and Escape Saddle Points** (Aug '18 - Mar '19) <br/>
    *Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay* <br/>
    * Proposed a **randomized iterative algorithm** to **detect** whether a critical point (i.e. a point where the derivatives of the loss function with respect to the parameters are zero) is a local minima or a **saddle point** and to **escape** that point if it is a saddle point, without requiring to compute the **Hessian**. <br/>
    * Essentially, the algorithm tries to find the direction corresponding to the **minimum eigenvalue of the Hessian** (without computing or storing it) by the use of **iid random samples** which leaves ample scope for **parallelization** of the computations involved in each iteration. <br/>
    * Its time complexity is **logarithmic wrt the dimension** and **approximately linear wrt the inverse of the magnitude of the minimum (negative) eigenvalue of the Hessian**. An upper bound for the number of random samples is also derived. <a href="https://drive.google.com/file/d/1Ecyn1ClyBC1lnpuCim0BxUskDfiFew-a/view" style="color: #0000FF">[Link]</a> <br/>
    
4.  **On the Existence of Sparse Bases for Deep Learning Kernels** (Aug '18 - Sep '18) <br/>
    *Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay* <br/>
    * Derived a probabilistic proof to suggest the possibility of the existence of sparse basis using few training points, for the final layer of binary classification networks before sigmoid (i.e. the transformed input which is linearly separable and the kernel being the transformation function) with the cross-entropy loss. The number of training points constituting the aforementioned sparse basis is much lesser than the dimension of the transformed input (or the dimension of the co-domain of the kernel function).<br/>
    * Hypothesis corroborated by experimental results. <br/>
    * This has an **important implication** - even though a large number of examples might be required to train deep learning networks, perhaps the **learnt kernel** can **generalize well** using only a **few of the training examples**. <a href="https://drive.google.com/file/d/1XnLKB8t8iNlR_PLlDJWXiMCkkRrCKP89/view" style="color: #0000FF">[Link]</a> <br/>
    
 5. **Sparse Kernel PCA (SKPCA) for Outlier Detection** (Nov '17 - May '18) <br/>
    *Guide : Prof. Suyash Awate, CSE Department, IIT Bombay* <br/>
    * Proposed a novel SKPCA algorithm by formulating it as a constrained optimization problem with elastic
      net regularization in the kernel space, solving it using alternating minimization. Tested it on 5 real world datasets and    showed that it outperforms the recent SKPCA method proposed in "Sparse kernel principal component analysis based on elastic net regularization." by Wang et al. (2016) which uses ADMM, with lesser parameter tuning. <br/>
    * Also presented a new probabilistic proof to justify the existence of sparse solutions in KPCA using the
      RBF kernel, which is the **first attempt** in this direction. <br/>
    * Paper accepted for **oral presentation** in **IEEE ICMLA 2018**. <a href="https://github.com/rudrajit15/Sparse-Kernel-PCA-for-outlier-detection/tree/master/skpca_codes" style="color: #0000FF">[Code]</a><br/>
    
 6. **Non-linear blind compressed sensing** (June '18 - Present) <br/>
    *Guide : Prof. Ajit Rajwade, CSE Department, IIT Bombay* <br/>
    * Working on an algorithm for non-linear blind compressed sensing (jointly estimating the sparse basis & sparse codes) which is a non-convex problem as well as its theoretical analysis which is an open problem. Currently focusing on the Anscombe transform (square root transform) for Poisson measurements. <br/>
    * Obtained a novel multiplicative update rule (like in NMF) to maintain positivity constraints of the sparse basis and
sparse codes. 
    * Currently working on deriving an upper bound on the algorithm’s expected value of the squared norm of the error (difference between the actual and estimated signal) using a Bernoulli sensing matrix and on the rate of decrease of the objective function with the number of iterations. <br/>
      
7. **Multiple Instance Learning (MIL) in Breast Cancer Histology Images** (Feb '18 - Present) <br/>
    *Guide : Prof. Amit Sethi, EE Department, IIT Bombay* <br/>
    * MIL is an unsupervised learning problem where the label of the entire image (“bag”) is given and the labels
      of the patches (“instances”) in the image are to be determined from this. <br/>
    * Currently working on self-supervised learning using the proxy tasks of colorization and novel gradient based
      segmentation (work in progress!), to learn good embeddings which can be used for deep attention based MIL. <br/>
    * Tried Bayesian Learning for MIL using features extracted from auto-encoders and obtained results comparable to state of
      the art for the Bisque data set. However, this method did not generalize well! <a href="https://github.com/rudrajit15/MIL-for-Breast-Cancer-Histology-Images/blob/master/Report/SRE_Report.pdf" style="color: #0000FF">[Report]</a> <br/>
      
8. **Sentence Compression Using Deep Learning** (Mar '18 - May '18) <br/>
    *Guide :  Prof. Sunita Sarawagi, CSE Department, IIT Bombay* <br/>
    * Designed a bi-directional 3-layer LSTM model for sentence compression by modelling it as a binary classification
      problem (which words to retain/delete). Compared it with the method proposed in “Sentence
      Compression by Deletion with LSTMs” by Google NLP Research and got marginally better results. <a href="https://github.com/rudrajit15/Sentence-Summarization-using-LSTMs/tree/master/Codes" style="color: #0000FF">[Code]</a> <a href="https://github.com/rudrajit15/Sentence-Summarization-using-LSTMs/blob/master/Report/AML%20Report.pdf" style="color: #0000FF">[Report]</a><br/>
    
9. **Speeding up Kernel PCA (KPCA)** (July '17 - Oct '17) <br/>
    *Guide : Prof. Suyash Awate, CSE Department, IIT Bombay* <br/>
    * Used the improved Nyström method to obtain a low rank approximation to the Gram matrix. Using this,
      developed a fast algorithm for eigenvector computation in KPCA, improving time complexity from $O(n^{2}p)$
      to $O(np^{2})$, where $n$ is the number of data points and $p \ll n$ is the rank of the approximated Gram matrix. <br/>
    * Simulated the above algorithm and obtained almost a linear speed up over MATLAB’s “eigs” function with
      negligible error in the obtained eigenvectors and eigenvalues. <a href="https://github.com/rudrajit15/Speeding-up-Kernel-PCA" style="color: #0000FF">[Code]</a> <a href="https://github.com/rudrajit15/Speeding-up-Kernel-PCA/blob/master/Report_Speeding_Up_KPCA.pdf" style="color: #0000FF">[Report]</a><br/>
     
**Research Internship :**   
 1. **Institute for Biomechanics, ETH Zürich, Switzerland** (May '17 - July '17) <br/>
    *Guide : Dr. Patrik Christen and Prof. Dr. Ralph Müller, D-HEST* <br/>
    * Constructed a linear model for bone re-modelling with some dependence on initial conditions, obtained a
      closed form solution for it and analyzed its stability using eigenvalue analysis, which was not done earlier. <br/>
    * Also built a directed graphical model to capture the random nature of the process and simulated it. <br/>
    * Developed an automated 2D-3D image registration framework for histology images from scratch, which
      included devising an efficient sampling strategy to obtain the 2D image across an arbitrary plane of the given
      3D image, formulating a good cost function (for measuring similarity) in order to mitigate the effect of the
      existence of several local minima, choosing a suitable optimization algorithm (tried Levenberg–Marquardt,
      Powell’s method, PSO, Genetic algorithms) and finally coding it all up. <br/>
      
I was also one of the very few undergraduates selected to attend the **PRAIRIE Artificial Intelligence Summer School** (<a href="https://project.inria.fr/paiss/" style="color: #0000FF">**PAISS**</a>) co-organized by Inria and NAVER LABS Europe in Grenoble, France during July 2018. Here I presented a poster (can be found <a href="https://github.com/rudrajit15/Existence-of-sparse-basis-for-deep-learning-kernels/blob/master/Inria_poster.pdf" style="color: #0000FF">here</a>) titled “**Existence of Sparse Basis for Deep Learning Kernels?**”.

**Key Academic Projects :**
1. **Using the Kernel Trick in Compressed Sensing** (April '18 - May '18) <br/>
    *Guide : Prof. Animesh Kumar, EE Department, IIT Bombay* <br/>
    * Implemented the paper “Using the kernel trick in compressive sensing: Accurate signal recovery from fewer
      measurements.” which performs compressed sensing in higher dimensional feature space by utilizing the
      kernel trick. The proposed method in the paper projects the data along random Gaussian directions and a
      probabilistic error bound is provided. <br/>
    * Extended the method to the case of directions sampled from a Bernoulli distribution, thus making it more
      hardware realizable. Also provided a theoretical proof for this extension. <a href="https://drive.google.com/file/d/1vCLvMuAeAQvw7ONtXrX6iTaR3POSz1lM/view?usp=sharing" style="color: #0000FF">[Report]</a> <a href="https://drive.google.com/file/d/1q6OYcockXVRTU2mm2J_DvEMRoHD6q_s2/view?usp=sharing" style="color: #0000FF">[Presentation]</a><br/>
      
2. **Extractive Text Summarization using Neural Networks** (Sep '17 - Nov '17) <br/>
    *Guide : Prof. Ganesh Ramakrishnan, CSE Department, IIT Bombay* <br/>
    * Implemented the paper “A Simple but Tough-to-Beat Baseline for Sentence Embeddings” and used the
      embeddings to select key sentences (modelled it as binary classification problem) in a document (extractive
      summarization) by ensembling neural networks. <br/>
    * Also designed a CNN architecture based on the EMNLP paper “Convolutional Neural Networks for Sentence
      Classification” which further improved results. <a href="https://github.com/rudrajit15/Document-Summarization" style="color: #0000FF">[Code]</a> <a href="https://github.com/rudrajit15/Document-Summarization/blob/master/Report.pdf" style="color: #0000FF">[Report]</a><br/>

3. **Image segmentation using Grab Cut Algorithm** (Feb '17 - April '17) <br/>
    *Guide : Prof. Suyash Awate, CSE Department, IIT Bombay* <br/>
    * Implemented Grab Cut which employs Gaussian Mixture Models (GMMs) along with the Graph Cut
      algorithm, for interactive extraction of foreground in a complex environment with reduced user interactions. <br/>
    * Simulated the algorithm on medical and natural images, obtaining good results. <a href="https://github.com/rudrajit15/Image-Segmentation-using-Grab-Cut" style="color: #0000FF">[Code]</a> <a href="https://github.com/rudrajit15/Image-Segmentation-using-Grab-Cut/blob/master/Report/MIP_Project_Report.pdf" style="color: #0000FF">[Report]</a><br/>
    
4. **Real Time Tracking of Non-Rigid Objects** (Feb '17 - April '17) <br/>
    *Guide : Prof. Ajit Rajwade, CSE Department, IIT Bombay* <br/>
    * Built a real time object tracking model for videos using mean shift algorithm with Bhattacharya coefficient
      to determine the object trajectory. It was robust to partial occlusion, clutter, rotation & camera position. <br/>
    * The model was successfully able to track humans, objects, vehicles etc. in real world videos. <a href="https://github.com/rudrajit15/Real-Time-Tracking-of-Non-Rigid-objects-using-Mean-Shift" style="color: #0000FF">[Code]</a> <a href="https://github.com/rudrajit15/Real-Time-Tracking-of-Non-Rigid-objects-using-Mean-Shift/blob/master/Report/CVProjectReport.pdf" style="color: #0000FF">[Report]</a><br/>

5. **Visible Light Communication(Li-Fi)** (Jan '17 - April '17) <br/>
    *Guide : Prof. Kumar Appaiah, EE Department, IIT Bombay* <br/>
    * Built an optical channel to transfer a Manchester encoded data stream synchronously. <br/>
    * Used Tiva-C micro-controller to transmit encoded data, which was received by a Clock Recovery Circuit;
      successfully decoded and displayed on an LCD at the receiving micro-controller.<br/>
    * Synchronously transferred encoded data at speed of 100 kbps over a distance of 3 meters. Also built an
      asynchronous system with a data rate of 30 kbps over 0.5 meters distance.<br/>
      
6. **Flow Based Image Extraction** (Sep '16 - Nov '16) <br/>
    *Guide : Prof. Suyash Awate & Ajit Rajwade, CSE Department, IIT Bombay* <br/>
    * Implemented a non-photorealistic rendering method to give stylized effect to images. <br/>
    * Applied a flow based difference of Gaussian filter for line extraction and then a flow based bilateral filter for
region smoothing to produce a stylized version of natural images. <a href="https://github.com/rudrajit15/Flow-Based-Image-Abstraction" style="color: #0000FF">[Code]</a> <br/>

7. **Min-cut based approach to find pathways in biological regulatory networks** (Dec '15 - Jan'16) <br/>
    *Guide : Prof. Supratik Chakraborty, CSE Department, IIT Bombay* <br/>
    * Worked on implementing an efficient semi-automated approach for finding pathways in systems biological
      regulatory networks using min-cuts. <br/>
    * Implemented the Gusfield algorithm in C++ to construct the Gomory Hu tree of the equivalent undirected
      graph which was used to obtain the min-cut edges between all pairs of nodes of the graph in $O(n)$ time,
      instead of the naive algorithm which takes $O(n^{2})$ time, thereby providing a linear speed up. <br/>
    * Also optimized the code in terms of memory by utilizing the sparsity of the adjacency matrix. <br/>
    
