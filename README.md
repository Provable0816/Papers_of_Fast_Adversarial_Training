# Papers_of_Fast_Adversarial_Training

+ Related Papers for Fast Adversarial Training

+ Stay updating… 

# Papers_of_Fast_Adversarial_Training


* [Understanding Catastrophic Overfitting in Adversarial Training](https://arxiv.org/abs/2105.02942) (done as a master thesis 2021)

* [Reliably fast adversarial training via latent adversarial perturbation](https://arxiv.org/abs/2104.01575) (ICCV 2021 Oral)
  * They deviate from the existing input-space-based adversarial training regime and propose a single-step latent adversarial training method (SLAT), which leverages the gradients of latent representation as the latent adversarial perturbation.

* [PGD-2 can be better than FGSM + GradAlign](https://openreview.net/forum?id=lifRwnIuAv0) (ICLR under review 2022)
  * [OpenReview](https://openreview.net/forum?id=lifRwnIuAv0)

* [ZeroGrad : Mitigating and Explaining Catastrophic Overfitting in FGSM Adversarial Training](https://arxiv.org/abs/2103.15476) (2021)
  * [code](https://github.com/rohban-lab/catastrophic_overfitting)
  * They support the idea that small input gradients play a key role in this phenomenon, and hence propose to zero the input gradient elements that are small for crafting FGSM attacks

* [Robust Single-step Adversarial Training with Regularizer](https://arxiv.org/abs/2102.03381) (2021)
  * They propose a novel Fast Gradient Sign Method with PGD Regularization (FGSMPR) to boost the efficiency of adversarial training without catastrophic overfitting. Their core idea is that single-step adversarial training can not learn robust internal representations of FGSM and PGD adversarial examples. Therefore, they design a PGD regularization term to encourage similar embeddings of FGSM and PGD adversarial examples

* [Recent Advances in Understanding Adversarial Robustness of Deep Neural Networks](https://arxiv.org/abs/2011.01539) (2020)
  * They give preliminary definitions on what adversarial attacks and robustness are. After that, they study frequently-used benchmarks and mention theoretically-proved bounds for adversarial robustness. They then provide an overview on analyzing correlations among adversarial robustness and other critical indicators of DNN models. Lastly, they introduce recent arguments on potential costs of adversarial training which have attracted wide attention from the research community.

* [Optimism in the Face of Adversity: Understanding and Improving Deep Learning through Adversarial Robustness](https://arxiv.org/abs/2010.09624) (2020)
  * They provide an in-depth review of the field of adversarial robustness in deep learning, and give a self-contained introduction to its main notions.
  *  The goal of this article is to provide readers with a set of new perspectives to understand deep learning, and to supply them with intuitive tools and insights on how to use adversarial robustness to improve it.

* [Understanding Catastrophic Overfitting in Single-step Adversarial Training](https://arxiv.org/abs/2010.01799) (AAAI 2021)
  * [code](https://github.com/Harry24k/catastrophic-overfitting)
  * They demonstrate that catastrophic overfitting is very closely related to the characteristic of single-step adversarial training which uses only adversarial examples with the maximum perturbation, and not all adversarial examples in the adversarial direction, which leads to decision boundary distortion and a highly curved loss surface. Based on this observation, this paper proposes a simple method that not only prevents catastrophic overfitting, but also overrides the belief that it is difficult to prevent multi-step adversarial attacks with single-step adversarial training.

* [Efficient Robust Training via Backward Smoothing](https://arxiv.org/abs/2010.01278) (2020) 
  * [code](https://github.com/uclaml/RayS)
  * [OpenReview](https://openreview.net/forum?id=49V11oUejQ)(Reject)
  * They show that the smoothing effect by random initialization is not sufficient under the adversarial perturbation constraint. A new initialization strategy, backward smoothing, is proposed to address this issue and significantly improves both stability and model robustness over single-step robust training methods.

* [Towards Understanding Fast Adversarial Training](https://arxiv.org/abs/2006.03089) (arxiv 2020)
  * [OpenReview](https://openreview.net/forum?id=NGBY716p1VR)(Reject)
  * They conduct experiments to understand the behavior of fast adversarial training and show the key to its success is the ability to recover from overfitting to weak attacks

* [Single-step Adversarial training with Dropout Scheduling](https://arxiv.org/abs/2004.08628) (CVPR 2020)
  *  (i) They show that models trained using single-step adversarial training method learn to prevent the generation of single-step adversaries, and this is due to over-fitting of the model during the initial stages of training, and (ii) to mitigate this effect, they propose a single-step adversarial training method with dropout scheduling

* [Understanding and Improving Fast Adversarial Training](https://arxiv.org/abs/2007.02617) (NeurIPS 2020) 
  * [code](https://github.com/tml-epfl/understanding-fast-adv-training)
  * GradAlign Method
  * They propose a new regularization method, GradAlign, that prevents catastrophic overfitting by explicitly maximizing the gradient alignment inside the perturbation set and improves the quality of the FGSM solution.

* [Fast is better than free: Revisiting adversarial training](https://arxiv.org/abs/2001.03994) (ICLR 2020) 
  * [code](https://github.com/locuslab/fast_adversarial)
  * They identify a failure mode referred to as “catastrophic overfitting” which may have caused previous attempts to use FGSM adversarial training to fail.

* [You Only Propagate Once: Accelerating Adversarial Training via Maximal Principle](https://arxiv.org/abs/1905.00877) (NeurIPS 2019)
  * [code](https://github.com/a1600012888/YOPO-You-Only-Propagate-Once)
  * In this paper, they show that adversarial training can be cast as a discrete time differential game. Through analyzing the Pontryagin's Maximal Principle (PMP) of the problem, they observe that the adversary update is only coupled with the parameters of the first layer of the network. This inspires us to restrict most of the forward and back propagation within the first layer of the network during adversary updates. This effectively reduces the total number of full forward and backward propagation to only one for each group of adversary updates

* [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843) (NeurIPS 2019)
  * [code](https://github.com/ashafahi/free_adv_train)
  * They present an algorithm that eliminates the overhead cost of generating adversarial examples by recycling the gradient information computed when updating model parameters.



* [Boosting Fast Adversarial Training with Learnable Adversarial Initialization](https://arxiv.org/abs/2110.05007) (TIP 2021) 
  * [code](https://github.com//jiaxiaojunQAQ//FGSM-SDI)
  * They boost fast AT with a sample-dependent adversarial initialization, i.e., an output from a generative network conditioned on a benign image and its gradient information from the target network.