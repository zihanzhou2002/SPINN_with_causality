# Instroduction
This is the github repository for the C6.5 Theories of Deep Learning Coursework Project *Physics-Informed Neural Networks: Tackling Complex
PDEs Through Dimension Separation and Causality* by Zihan Zhou. The project report is available at `ZihanZhou_report.pdf`. This repository is forked from [Junwoo Cho's original repo](https://github.com/stnamjef/SPINN) for his paper  [*Separable physics-informed neural networks*](https://arxiv.org/abs/2306.15969), published at Conference on Neural Information Processing Systems (NeurIPS 2023).

# Main Contribution
This report investigates the introduction of causality into Separable Physics-Informed Neural Networks(SPINN), and tested the effect on Klein-Gordon equation and diffusion equation. THe relevant codes are available at `diffusion3d_causal.py` and `causal_spinn_kleingordon.ipynb`, and the set of causality parameter we used are `[1e-3, 1e-2, 1e-1, 1]`. The results are summarised in the `Causal_results_KleinGordon` and `causal_results_diffusion` folders.

SPINN with causality achieves promising results on the Klein-Gordon equation, but experiments show that the introduction of causality disrupts the diffusion process. Below is an example of the diffusion process when causality prameter $\epsilon = 1$.

![pred_0 1](https://github.com/user-attachments/assets/d06dd381-6841-4081-8849-25a9c0c9a516)
![pred_1 0](https://github.com/user-attachments/assets/85b2703b-da52-4c3f-aa86-a2998d01f86d)
