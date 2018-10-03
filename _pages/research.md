---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
use_math: true
---
**Research Experience :**
1.  **Improving Optimization in Deep Learning - Master’s Thesis** (June '18 - Present) <br/>
    *Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay* <br/>
    * As of now, proposed a novel randomized iterative algorithm to detect whether a critical point (i.e. a point where the
    derivatives of the loss function with respect to the parameters are zero) is a local minima or a saddle point
    and to escape that point if it is a saddle point, without requiring to compute the Hessian. <br/>
    * Derived an upper bound on the expected number of iterations, which is logarithmic with respect to the
    number of positive eigenvalues of the Hessian at that point and faster than linearithmic with respect to
    the inverse of the magnitude of the minimum eigenvalue of the Hessian. The **complexity wrt the minimum
    eigenvalue of the Hessian is better** than that of Perturbed Gradient Descent (PGD) proposed in "How to escape saddle points efficiently." by Jin et al. (2017) and CNC-GD proposed in "Escaping Saddles with Stochastic
    Gradients." by Daneshmand et al. (2018). <br/>
    * Also, in relation to the complexity of the proposed algorithm, obtained approximate upper and lower bounds
    for the expected number of negative eigenvalues of the Hessian (known as the index) at a point, as a function
    of the loss value at that point, for a single hidden layer neural network with the cross-entropy loss function.
    This is the **first attempt at index computation for the cross-entropy loss function**. <br/>
    * Paper submitted to **AAAI-19**. <br/>
    
2.  **Existence of Sparse Basis for Kernels of Binary Classification Networks? - Master’s Thesis** (Sep '18 - Present) <br/>
    *Guide : Prof. Subhasis Chaudhuri, EE Department, IIT Bombay* <br/>
    * Derived a probabilistic proof to suggest the possibility of the existence of sparse basis using few training points, for the final layer of binary classfication networks before sigmoid (i.e. the transformed input which is linearly separable and the kernel being the transformation function) with the cross-entropy loss. The number of training points constituting the aforementioned sparse basis is much lesser than the dimension of the transformed input (or the dimension of the co-domain of the kernel function).<br/>
    * Hypothesis corroborated by experimental results. <br/>
    * This has an **important implication** - even though a large number of examples might be required to train deep learning networks, perhaps the **learnt kernel** can **generalize well** using only a **few of the training examples**. <br/>
    * Paper submitted to **AAAI-19**. <br/>
    
 3. **Sparse Kernel PCA (SKPCA) for Outlier Detection** (Nov '17 - May '18) <br/>
    *Guide : Prof. Suyash Awate, CSE Department, IIT Bombay* <br/>
    * Proposed a novel SKPCA algorithm by formulating it as a constrained optimization problem with elastic
      net regularization in the kernel space, solving it using alternating minimization. Tested it on 5 real world datasets and    showed that it outperforms the recent SKPCA method proposed in "Sparse kernel principal component analysis based on elastic net regularization." by Wang et al. (2016) which uses ADMM, with lesser parameter tuning. <br/>
    * Also presented a new probabilistic proof to justify the existence of sparse solutions in KPCA using the
      RBF kernel, which is the **first attempt** in this direction. <br/>
    * Paper accepted for **oral presentation** in **IEEE ICMLA 2018**. <a href="https://github.com/rudrajit15/Sparse-Kernel-PCA-for-outlier-detection/tree/master/skpca_codes" style="color: #0000FF">[Code]</a><br/>
    
 4. **Non-linear blind compressed sensing** (June '18 - Present) <br/>
    *Guide : Prof. Ajit Rajwade, CSE Department, IIT Bombay* <br/>
    * Working on an algorithm for blind compressed sensing (jointly estimating the sparse basis & sparse codes) under non-linear
      transformations of data to make the noise model Gaussian, such as the Anscombe transform for Poisson
      measurements. This has not been done before and is challenging due to the non-linearity and the highly
      non-convex nature of the problem. <br/>
    * Obtained an upper bound on the algorithm's expected value of the squared norm of the error (difference between the actual signal and estimated signal) using a Bernoulli sensing matrix, as a function of the ratio of the number of measurements to signal dimension, number of training examples and value of the squared loss part of the objective function. <br/>
      
5. **Multiple Instance Learning (MIL) in Breast Cancer Histology Images** (Feb '18 - Present) <br/>
    *Guide : Prof. Amit Sethi, EE Department, IIT Bombay* <br/>
    * MIL is an unsupervised learning problem where the label of the entire image (“bag”) is given and the labels
      of the patches (“instances”) in the image are to be determined from this. <br/>
    * Currently working on self-supervised learning using the proxy tasks of colorization and novel gradient based
      segmentation (work in progress!), to learn good embeddings which can be used for deep attention based MIL. <br/>
    * Tried Bayesian Learning for MIL using features extracted from auto-encoders and obtained results comparable to state of
      the art for the Bisque data set. However, this method did not generalize well! <a href="https://github.com/rudrajit15/MIL-for-Breast-Cancer-Histology-Images/blob/master/Report/SRE_Report.pdf" style="color: #0000FF">[Report]</a> <br/>
      
6. **Sentence Compression Using Deep Learning** (Mar '18 - May '18) <br/>
    *Guide :  Prof. Sunita Sarawagi, CSE Department, IIT Bombay* <br/>
    * Designed a bi-directional 3-layer LSTM model for sentence compression by modelling it as a binary classification
      problem (which words to retain/delete). Compared it with the method proposed in “Sentence
      Compression by Deletion with LSTMs” by Google NLP Research and got marginally better results. <a href="https://github.com/rudrajit15/Sentence-Summarization-using-LSTMs/tree/master/Codes" style="color: #0000FF">[Code]</a> <a href="https://github.com/rudrajit15/Sentence-Summarization-using-LSTMs/blob/master/Report/AML%20Report.pdf" style="color: #0000FF">[Report]</a><br/>
    
7. **Speeding up Kernel PCA (KPCA)** (July '17 - Oct '17) <br/>
    *Guide : Prof. Suyash Awate, CSE Department, IIT Bombay* <br/>
    * Used the improved Nyström method to obtain a low rank approximation to the Gram matrix. Using this,
      developed a fast algorithm for eigenvector computation in KPCA, improving time complexity from $O(n^{2}p)$
      to $O(np^{2})$, where n is the number of data points and p << n is the rank of the approximated Gram matrix. <br/>
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
    
