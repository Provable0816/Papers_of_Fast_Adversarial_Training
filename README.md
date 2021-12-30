# Papers_of_Fast_Adversarial_Training

+ Related Papers for Fast Adversarial Training

+ stay updating

# Conference_Papers_of_Fast_Adversarial_Training

* [Understanding and Improving Fast Adversarial Training](https://arxiv.org/abs/2007.02617) (NeurIPS 2020) 
  * [code](https://github.com/tml-epfl/understanding-fast-adv-training)
  * GradAlign Method
  * This paper proposes a new regularization method, GradAlign, that prevents catastrophic overfitting by explicitly maximizing the gradient alignment inside the perturbation set and improves the quality of the FGSM solution.
* [Towards Understanding Fast Adversarial Training](https://arxiv.org/abs/2006.03089) (arxiv 2020)
  *  This paper conducts experiments to understand the behavior of fast adversarial training and show the key to its success is the ability to recover from overfitting to weak attacks
  * 
* [Fast is better than free: Revisiting adversarial training](https://arxiv.org/abs/2001.03994) (ICLR 2020) 
  * [code](https://github.com/locuslab/fast_adversarial)
  * This paper identifies a failure mode referred to as “catastrophic overfitting” which may have caused previous attempts to use FGSM adversarial training to fail.
  * 
* [Adversarial Training for Free!](https://arxiv.org/abs/1904.12843) ( NeurIPS 2019)
  * [code](https://github.com/ashafahi/free_adv_train)
  * This paper presents an algorithm that eliminates the overhead cost of generating adversarial examples by recycling the gradient information computed when updating model parameters.


# Transactions_Papers_of_Fast_Adversarial_Training

* [Boosting Fast Adversarial Training with Learnable Adversarial Initialization](https://arxiv.org/abs/2110.05007) (TIP 2021) 
  * [code](https://github.com//jiaxiaojunQAQ//FGSM-SDI)
  * This paper boosts fast AT with a sample-dependent adversarial initialization, i.e., an output from a generative network conditioned on a benign image and its gradient information from the target network.