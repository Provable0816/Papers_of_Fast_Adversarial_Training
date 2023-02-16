# Papers_of_Fast_Adversarial_Training

+ Related Papers for Fast Adversarial Training

+ Stay updating… 

# Contents 
- <a href="#Papers_of_Fast_Adversarial_Training"> Papers_of_Fast_Adversarial_Training</a><br>
- <a href="#Unfair problem in Adversarial Training">Unfair problem in Adversarial Training</a><br>



<a id='Papers_of_Fast_Adversarial_Training'></a>
## Papers_of_Fast_Adversarial_Training


* [Prior-Guided Adversarial Initialization for Fast Adversarial Training](https://arxiv.org/abs/2207.08859)
  * [code](https://github.com/jiaxiaojunqaq/fgsm-pgi)
  * They explore the difference between the training processes of SAT and FAT and observe that the attack success rate of adversarial examples (AEs) of FAT gets worse gradually in the late training stage, resulting in overfitting. They propose a prior-guided FGSM initialization method to avoid overfitting after investigating several initialization strategies, improving the quality of the AEs during the whole training process. The initialization is formed by leveraging historically generated AEs without additional calculation cost.


* [Revisiting and Advancing Fast Adversarial Training Through The Lens of Bi-Level Optimization](https://arxiv.org/abs/2112.12376)
  * [OpenReview](https://openreview.net/forum?id=gzeruP-0J29)
  * [code](https://github.com/normaluhr/fast_bat)
  * They propose to design FAST-AT from the perspective of bi-level optimization (BLO). They first make the key observation that the most commonly-used algorithmic specification of FAST-AT is equivalent to using some gradient descent-type algorithm to solve a bi-level problem involving a sign operation. However, the discrete nature of the sign operation makes it difficult to understand the algorithm performance. Based on the above observation, they propose a new tractable bi-level optimization problem, design and analyze a new set of algorithms termed Fast Bi-level AT (FAST-BAT). FAST-BAT is capable of defending sign-based projected gradient descent (PGD) attacks without calling any gradient sign method and explicit robust regularization. Furthermore, they empirically show that their method outperforms state-of-the-art FAST-AT baselines, by achieving superior model robustness without inducing robustness catastrophic overfitting, or suffering from any loss of standard accuracy.

* [ℓ∞ -Robustness and Beyond: Unleashing Efficient Adversarial Training](https://arxiv.org/abs/2112.00378) 
  * [OpenReview](https://openreview.net/forum?id=zfKQn4zN6sB)
  * In this paper, by leveraging the theory of coreset selection they show how selecting a small subset of training data provides a more principled approach towards reducing the time complexity of robust training. Unlike existing methods, their approach can be adapted to a wide variety of training objectives, including TRADES, ℓp-PGD, and Perceptual Adversarial Training. Their experimental results indicate that our approach speeds up adversarial training by 2-3 times, while experiencing a small reduction in the clean and robust accuracy.

* [Subspace Adversarial Training](https://arxiv.org/abs/2111.12229)
  * [code](https://github.com/nblt/Sub-AT) (404 not found)
  * To control the growth of the gradient during the training, they propose a new AT method, subspace adversarial training (Sub-AT), which constrains the AT in a carefully extracted subspace. It successfully resolves both two kinds of overfitting and hence significantly boosts the robustness. In subspace, they also allow single-step AT with larger steps and larger radius, which further improves the robustness performance. 

* [Local Linearity and Double Descent in Catastrophic Overfitting](https://arxiv.org/abs/2111.10754) (CODS-COMAD 2022)
  * [code](https://github.com/nikilrselvam/linearity-orthogonality-dd) (waitting for code)
  * They experimentally demonstrate that maintaining high local linearity might be sufficient to prevent catastrophic overfitting but is not necessary. Further, inspired by Parseval networks, they introduce a regularization term to AT with FGSM to make the weight matrices of the network orthogonal and study the connection between orthogonality of the network weights and local linearity. Lastly, they identify the double descent phenomenon during the adversarial training process.  

* [Towards Efficient and Effective Adversarial Training](https://neurips.cc/Conferences/2021/ScheduleMultitrack?event=26270) (NeurIPS 2021)
  * [OpenReview](https://openreview.net/forum?id=kuK2VARZGnI)
  * [code](https://github.com/val-iisc/NuAT)(waitting for code)
  * They bridge this performance gap by introducing a novel Nuclear-Norm regularizer on network predictions to enforce function smoothing in the vicinity of data samples.  While prior works consider each data sample independently, the proposed regularizer uses the joint statistics of adversarial samples across a training minibatch to enhance optimization during both attack generation and training, obtaining state-of-the-art results amongst efficient defenses. They achieve further gains by incorporating exponential averaging of network weights over training iterations. They finally introduce a Hybrid training approach that combines the effectiveness of a two-step variant of the proposed defense with the efficiency of a single-step defense. They demonstrate superior results when compared to multi-step defenses such as TRADES and PGD-AT as well, at a significantly lower computational cost.

* [Boosting Fast Adversarial Training with Learnable Adversarial Initialization](https://arxiv.org/abs/2110.05007) (TIP 2021) 
  * [code](https://github.com//jiaxiaojunQAQ//FGSM-SDI)
  * They boost fast AT with a sample-dependent adversarial initialization, i.e., an output from a generative network conditioned on a benign image and its gradient information from the target network.

* [Understanding Catastrophic Overfitting in Adversarial Training](https://arxiv.org/abs/2105.02942) (done as a master thesis 2021)

* [Reliably fast adversarial training via latent adversarial perturbation](https://arxiv.org/abs/2104.01575) (ICCV 2021 Oral)
  * They deviate from the existing input-space-based adversarial training regime and propose a single-step latent adversarial training method (SLAT), which leverages the gradients of latent representation as the latent adversarial perturbation.

* [PGD-2 can be better than FGSM + GradAlign](https://openreview.net/forum?id=lifRwnIuAv0) (ICLR under review 2022)
  * [OpenReview](https://openreview.net/forum?id=lifRwnIuAv0)

* [Gradient-Guided Dynamic Efficient Adversarial Training](https://arxiv.org/abs/2103.03076) 
  * [code](https://github.com/locuslab/fast_adversarial)
  * They propose the Dynamic Efficient Adversarial Training (DEAT), which gradually increases the adversarial iteration during training. Moreover, they theoretically reveal that the connection of the lower bound of Lipschitz constant of a given network and the magnitude of its partial derivative towards adversarial examples. Supported by this theoretical finding, they utilize the gradient's magnitude to quantify the effectiveness of adversarial training and determine the timing to adjust the training procedure

* [ZeroGrad : Mitigating and Explaining Catastrophic Overfitting in FGSM Adversarial Training](https://arxiv.org/abs/2103.15476) (2021)
  * [code](https://github.com/rohban-lab/catastrophic_overfitting)
  * They support the idea that small input gradients play a key role in this phenomenon, and hence propose to zero the input gradient elements that are small for crafting FGSM attacks

* [Robust Single-step Adversarial Training with Regularizer](https://arxiv.org/abs/2102.03381) (2021)
  * They propose a novel Fast Gradient Sign Method with PGD Regularization (FGSMPR) to boost the efficiency of adversarial training without catastrophic overfitting. Their core idea is that single-step adversarial training can not learn robust internal representations of FGSM and PGD adversarial examples. Therefore, they design a PGD regularization term to encourage similar embeddings of FGSM and PGD adversarial examples

* [Guided Adversarial Attack for Evaluating and Enhancing Adversarial Defenses](https://arxiv.org/abs/2011.14969)
  * [code](https://github.com/val-iisc/GAMA-GAT)
  * They introduce a relaxation term to the standard loss, that finds more suitable gradient-directions, increases attack efficacy and leads to more efficient adversarial training. They propose Guided Adversarial Margin Attack (GAMA), which utilizes function mapping of the clean image to guide the generation of adversaries, thereby resulting in stronger attacks. They evaluate our attack against multiple defenses and show improved performance when compared to existing attacks. Further, They propose Guided Adversarial Training (GAT), which achieves state-of-the-art performance amongst single-step defenses by utilizing the proposed relaxation term for both attack generation and training.

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

* [Understanding and Improving Fast Adversarial Training](https://arxiv.org/abs/2007.02617) (NeurIPS 2020) 
  * [code](https://github.com/tml-epfl/understanding-fast-adv-training)
  * GradAlign Method -- Using cosine similarity to measure the distance of the logit of natural examples and adversarial examples
  * They propose a new regularization method, GradAlign, that prevents catastrophic overfitting by explicitly maximizing the gradient alignment inside the perturbation set and improves the quality of the FGSM solution.

* [Towards Understanding Fast Adversarial Training](https://arxiv.org/abs/2006.03089) (arxiv 2020)
  * [OpenReview](https://openreview.net/forum?id=NGBY716p1VR)(Reject)
  * They conduct experiments to understand the behavior of fast adversarial training and show the key to its success is the ability to recover from overfitting to weak attacks

* [Single-step Adversarial training with Dropout Scheduling](https://arxiv.org/abs/2004.08628) (CVPR 2020)
  *  (i) They show that models trained using single-step adversarial training method learn to prevent the generation of single-step adversaries, and this is due to over-fitting of the model during the initial stages of training, and (ii) to mitigate this effect, they propose a single-step adversarial training method with dropout scheduling

* [Fast is better than free: Revisiting adversarial training](https://arxiv.org/abs/2001.03994) (ICLR 2020) 
  * [code](https://github.com/locuslab/fast_adversarial)
  * They identify a failure mode referred to as “catastrophic overfitting” which may have caused previous attempts to use FGSM adversarial training to fail.

* [You Only Propagate Once: Accelerating Adversarial Training via Maximal Principle](https://arxiv.org/abs/1905.00877) (NeurIPS 2019)
  * [code](https://github.com/a1600012888/YOPO-You-Only-Propagate-Once)
  * In this paper, they show that adversarial training can be cast as a discrete time differential game. Through analyzing the Pontryagin's Maximal Principle (PMP) of the problem, they observe that the adversary update is only coupled with the parameters of the first layer of the network. This inspires us to restrict most of the forward and back propagation within the first layer of the network during adversary updates. This effectively reduces the total number of full forward and backward propagation to only one for each group of adversary updates

* [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843) (NeurIPS 2019)
  * [code](https://github.com/ashafahi/free_adv_train)
  * They present an algorithm that eliminates the overhead cost of generating adversarial examples by recycling the gradient information computed when updating model parameters.


<a id='Unfair problem in Adversarial Training'></a>
## Unfair problem in Adversarial Training

* [Understanding the robustness-accuracy tradeoff by rethinking robust fairness](https://openreview.net/forum?id=bl9zYxOVwa)

* [Analysis and Applications of Class-wise Robustness in Adversarial Training](https://arxiv.53yu.com/abs/2105.14240)

* [To be Robust or to be Fair: Towards Fairness in Adversarial Training](https://arxiv.org/abs/2010.06121)

* [#TODO]