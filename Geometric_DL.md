# Geometric DL
2020.12.22

[PROFESSOR MICHAEL BRONSTEIN](https://www.imperial.ac.uk/people/m.bronstein)<br>

* [2020: Товарищ Бронштейн: Do we need deep graph neural networks?](https://towardsdatascience.com/do-we-need-deep-graph-neural-networks-be62d3ec5c59)

 -- This year, deep learning on graphs was crowned among the hottest topics in machine learning.

 -- Training deep graph neural networks is hard. Besides the standard plights observed in deep neural architectures such as vanishing gradients in back-propagation and overfitting due to a large number of parameters, there are a few problems specific to graphs. One of them is over-smoothing, the phenomenon of the node features tending to converge to the same vector and become nearly indistinguishable as the result of applying multiple graph convolutional layers [1].

 -- This behaviour was first observed in GCN models [2,3], which act similarly to low-pass filters.

 -- Another phenomenon is a bottleneck, resulting in “over-squashing” of information from exponentially many neighbours into fixed-size vectors [4].

 -- ... problem of depth in graph neural networks, in hope to achieve better performance and perhaps avoid embarrassment in using the term “deep learning” when referring to graph neural networks with just two layers. 


 -- Typical approaches can be split into two families. First, regularisation techniques such as edge-wise dropout (DropEdge) [5], pairwise distance normalisation between node features (PairNorm) [6], or node-wise mean and variance normalisation (NodeNorm) [7]. Second, architectural changes including various types of residual connection such as jumping knowledge [8] or affine residual connection [9]. 

 -- the use of deep architectures often results in decreased performance.



* [2017 Geometric deep learning: going beyond Euclidean data; M.Bronstein, J.Bruna, Yann LeCun, A.Szlam, P.Vandergheynst; arxiv.org/abs/1611.08097](https://arxiv.org/pdf/1611.08097.pdf)<br>

      The purpose of this paper is to overview different examples of geometric deep learning problems and present available 
      solutions, key difficulties, applications, and future research directions in this nascent field.
* [2020:YT: Geometric Deep Learning - Michael Bronstein - MLSS 2020, Tübingen](https://www.youtube.com/watch?v=8kTxTX0eBRA)<br>

      conv filter = tri-diagonal matrix multiplication = lin comb of weighted shifts of adj matrix
      32:11 Graph ConvNet: Y = ReLU ( AXW )
             Y = SoftMax( A ReLU ( AXW1 ) W2 )
      39:42 For what graphs do we need depth?
            For in computer vision NNs are deep, 100+ layers. For graphs usually - NO.

[Alex Bronstein](https://bron.cs.technion.ac.il/)<br>
* [2019: Learning deformable shape correspondence](http://www.ipam.ucla.edu/abstract/?tid=15397&pcode=GLWS2)<br>
     
       Functional Correspondence in Spectral Domain
* [2020: Deep Matrix Factorization with Spectral Geometric Regularization, Boyarski, Vedula, A.Bronstein arxiv.org/pdf/1911.07255.pdf](https://arxiv.org/pdf/1911.07255.pdf)<br>
     * [COLAB CODE OF SGMC Toy Example](https://github.com/ftk1000/GraphNeuralNets/blob/main/SGMC_toy_example.ipynb)<br>     
     * [synthetic_netflix.mat - Data file for the Toy Example](https://github.com/ftk1000/GraphNeuralNets/blob/main/synthetic_netflix.mat)<br>
     * [importing-data-to-google-colab-the-clean-way](https://towardsdatascience.com/importing-data-to-google-colab-the-clean-way-5ceef9e9e3c8)<br>
     
[]()<br>

        Tula, Russia 1980
        Table of Contents (powered by https://videoken.com)
        0:00:00 Speaker Introduction
        0:02:04 Geometric Deep Learning - going beyond Euclidean data
        0:02:36 Motivation
        0:02:48 Perceptron
        0:03:03 Multilayer perceptron
        0:03:20 Multilayer perceptron = universal approximator
        0:03:57 Curse of dimensionality
        0:05:31 Computer vision problems
        0:06:17 Take advantage of structure!
        0:06:54 Convolutional Neural Networks
        0:07:35 Inductive biases
        0:08:20 energy U = ?
        0:10:43 Geometric Deep Learning
        0:10:57 Prototypical objects
        0:11:16 Images and Graphs
        0:12:24 Convolution
        0:12:38 Fully connected layer
        0:13:06 Sparsely connected layer
        0:13:21 Convolutional layer
        0:14:24 Shift-equivariance
        0:14:43 Joint diagonalization
        0:15:03 Eigenvectors of ST = Fourier transform
        0:15:15 Convolution in spectral domain
        0:15:36 Convolution theorem
        0:16:13 Key insights
        0:17:12 From grids to graphs
        0:17:15 Graphs
        0:17:47 Attributes
        0:18:12 Adjacently matrix
        0:18:22 Weighted adjacently matrix
        0:18:39 Graph Laplacian
        0:19:23 Dirichlet energy
        0:19:45 Laplacian on manifolds and meshes
        0:20:28 Convolution on graphs?
        0:20:53 Graph Fourier transform
        0:21:03 1D grid = ring graph
        0:21:30 From Grid to Graph Fourier Transform
        0:22:52 Spectral graph convolution
        0:24:32 Spectral graph convolution: drawbacks
        0:24:54 Basis dependence
        0:25:45 Isotropic filters on graphs
        0:26:38 Anisotropic filters on meshes
        0:27:14 Spectral graph convolution, take 2
        0:28:16 Polynomial filter (ChebNet)
        0:29:46 Spatial graph convolution
        0:30:09 Convolution, revisited
        0:31:01 Graph Convolutional Networks (GCN)
        0:33:03 Pooling
        0:33:10 Graph coarsening
        0:34:11 Deep graph neural networks
        0:34:25 Challenges of going deep on graphs
        0:35:33 Does depth help?
        0:36:41 Simplified GCN (SGCN)
        0:37:21 SIGN: Scalable Inception-like Graph Neural network
        0:38:30 SIGN scalability
        0:39:01 Do we need depth for graphs?
        0:39:35 For what graphs do we need depth?
        0:43:06 Different recipes for graph convolution
        0:43:53 MoNet
        0:44:24 Graph Attention Networks (GAT)
        0:45:14 Message Passing Neural Network (MPNN)
        0:46:19 How powerful are graph neural networks?
        0:46:55 Graph isomorphism
        0:47:47 Weisfeiler-Lehman test
        0:49:20 How powerful is WL test?
        0:49:57 Message passing and WL tests
        0:53:05 How powerful are GSN?
        0:54:09 What substructure to use?
        0:54:37 Substructures in chemistry
        0:55:34 Theory beyond Weisfeiler-Lehman
        0:57:08 What's next?
        0:58:16 The road ahead
        1:00:51 Dynamic graphs
        1:01:22 Temporal Graph Networks
        1:02:01 Higher-order structures
        1:03:58 Robustness and guaranteed performance
        1:05:21 ICLR 2020 submissions keyword statistics
        1:05:44 Graphs = systems of relations and interactions
        1:08:10 Recommender systems and link prediction
        1:09:01 Learning the graph
        1:10:32 High-energy physics
        1:11:30 Neutrino detection
        1:12:22 Computational chemistry and drug design
        1:14:26 Hyperfoods
        1:16:59 Combinatorial drug therapy
        1:18:42 Protein science and cancer immunotherapy
        1:19:17 De novo protein design
        1:20:15 3D vision and graphics
        1:20:55 Shape analysis and synthesis
        1:21:15 Classical and Geometric (intrinsic) convolution
        1:21:46 Deformable shape correspondence
        1:22:01 3D generative models
        1:22:24 3D hand reconstruction from 2D images
        1:23:33 CVPR 2020 = Geometry + Deep Learning
        1:24:12 Conclusions
        1:25:54 Q&A
