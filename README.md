# Generative-Models
Implementations of several generative models from scratch.

## CycleGAN


The cycle-consistent generative adversarial network (CycleGAN) is a type of artiﬁcial neural network that is capable of performing image-to-image translations. It is capable of doing this translation when paired data is not available for training. CycleGAN uses 2 generators and two discriminators. 
### Architecture
The model contains two mapping functions G : X → Y and F : Y → X, and associated adversarial discriminators D_Y and D_X. D_Y encourages G to translate X into outputs indistinguishable from domain Y, and vice versa for D_X and F. Two cycle consistency losses: (b) forward cycle-consistency loss: x → G(x) → F (G(x)) ≈ x, and (c) backward cycle-consistency loss: y → F (y) → G(F (y)) ≈ y
#### Generator
#### Discriminator

### Details

#### Instance Normalisation
Acording to Andrew NG's course, Batch Normalisation helps in faster training by turning the activation towards unit Gaussian distribution and thus tackling vanishing gradients problem.
Instance normalisation, on the other hand, acts as contrast normalisation as mentioned in the [paper][CycleGAN Paper]. The intuition behind this is that the results should not depend on the contrast of input image.
#### Patch GAN

#### Convolution Transpose


[CycleGAN Paper]: https://arxiv.org/pdf/1703.10593.pdf
[Patch GAN Paper]: https://arxiv.org/pdf/1611.07004.pdf
[]: https://towardsdatascience.com/cyclegan-learning-to-translate-images-without-paired-training-data-5b4e93862c8d
