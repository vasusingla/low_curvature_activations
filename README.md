
### Low Curvature Activations Reduce Overfitting in Adversarial Training 
Implementation and experiments fo the paper low curvature activations reduce robust overfitting.

It has been shown that for adversarial training robust accuracy decreases as you train longer [1].
In our work, we show that choice of activation function has a significant impact on the robust overfitting
phenomenon and the double  descent generalization curves. For more details read our paper on [arxiv][arxiv_paper_link].

This repository was forked over and implemented from original implementation of the robust overfitting paper
[here][original_repo_link]. 

To run experiments with different activation functions, for CIFAR-10 -  \
<code>
python  train_cifar.py --activation \<specify_act_fn></code>

To run experiments with different activation functions, for CIFAR-10 -  \
<code>
python  train_cifar100.py --activation \<specify_act_fn></code>

Use <code>generate_validation.py</code> to generate validation dataset, and specify <code>--val</code> flag to run
experiments with validation dataset. All the activation functions considered in the paper, and several more are listed
in train_cifar.py <code>--activation</code> flag.

If you find our work useful, please consider citing -

```
@misc{singla2021low,
      title={Low Curvature Activations Reduce Overfitting in Adversarial Training}, 
      author={Vasu Singla and Sahil Singla and David Jacobs and Soheil Feizi},
      year={2021},
      eprint={2102.07861},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```


**References**

\[1] [Overfitting in adversarially robust deep learning][overfitting_paper] 

[arxiv_paper_link]: https://arxiv.org/abs/2102.07861
[overfitting_paper]: https://arxiv.org/abs/2002.11569
[original_repo_link]: https://github.com/locuslab/robust_overfitting