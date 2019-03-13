
### Quantization

1. [The ZipML Framework for Training Models with End-to-End Low Precision: The Cans, the Cannots, and a Little Bit of Deep Learning](https://arxiv.org/abs/1611.05402) [ICML'17]

  recently there has been significant interest in training nueral net works in low presision: by reducing presision, one can reduce computation and communication by one order of  magnitude.
  We examine traning in reduced precision, both from theoratical and practical perspective, and ask: is it possible to train models at end-to-end low precision with provalble guarantees?
  Can this lead to consistent order-of-maganitude speed up?
  We present a framework named ZipML to answer these questions. For linear models , the answer is yes . We develop a simple framework based on one simple but novel stratigy called double sampling. 
  Our framework is able to excute in low precision with no bias, guaranteeing convergence, where as naive low precision methods lead to significant bias.
  We validate our framework across a range of application, and show that it enables an FPGA prototype that is up to 6.5X faster than an implementation using full 32-bit single precision. 
  We further develop a variance-optimal stochastic quantization stratiegy and show that it can make sinificant difference in a variaty of settings. When applied on linear models together with double sampling, we save up to another 1.7X in data movement compared with unifrom qauntization.
  When training deep networks with quantized models, we achive higher accuracy than the state of art XNOR net.Finally ,we extened or framework through approximation to non-linear models, such as SVM.
  We show that, although using lower precision data includes bias, we can appropriately bound and control the bias.We find in practice 8-bit precision is often sufficient to converge to the correct solution.Interestingly, however, in practice we find that our frameworks does not always outperform the native rouding approach. We discuss this negative result in detail.
1. [Compressing Deep Convolutional Networks using Vector Quantization](https://arxiv.org/abs/1412.6115) [arXiv'14]

Deep convolutional neural net work has become the most promising  method for object detection,
rapeatedly demortrating record breaking the results for image classidication and object 
detection in recent years.
However, a very deep CNN generally involves many layers woth millions of parameters, making the 
storage of the net work model to be extremely large . This prohibits the usage of deep CNNs 
on resourse limited platforms , espetailly cell phones and  other embedded devices.In this paper 
we tackel this storage issue by investigating information theoreticle vector quantization 
methods for compressing the parameters of CNNs. In paticular ,we have found in terms of 
compressing the most storage demanding dense connected layers ,vector quantization method have
a clear gain over existing matrix factorazition method. Simply apply K-means clustering to the 
weights or conducting product quantization can lead to a very good balance between model size
and recognotion accuracy.For the 1000-category classification task in Image-Net Challage ,we are able to 
achive 16-24 times compression of the network with only 1% loss of the classfication accuracy using 
the state-of-art CNN.

1. [Quantized Convolutional Neural Networks for Mobile Devices](https://arxiv.org/abs/1512.06473) [CVPR '16]
1. [Fixed-Point Performance Analysis of Recurrent Neural Networks](https://arxiv.org/abs/1512.01322) [ICASSP'16]
1. [Quantized Neural Networks: Training Neural Networks with Low Precision Weights and Activations](https://arxiv.org/abs/1609.07061) [arXiv'16]
1. [Loss-aware Binarization of Deep Networks](https://arxiv.org/abs/1611.01600) [ICLR'17]
1. [Towards the Limit of Network Quantization](https://arxiv.org/abs/1612.01543) [ICLR'17]
1. [Deep Learning with Low Precision by Half-wave Gaussian Quantization](https://arxiv.org/abs/1702.00953) [CVPR'17]
1. [ShiftCNN: Generalized Low-Precision Architecture for Inference of Convolutional Neural Networks](https://arxiv.org/abs/1706.02393) [arXiv'17]
1. [Training and Inference with Integers in Deep Neural Networks](https://openreview.net/forum?id=HJGXzmspb) [ICLR'18]
1. [Deep Learning with Limited Numerical Precision](https://arxiv.org/abs/1502.02551)[ICML'2015]
