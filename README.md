## MC-PILCO: Monte Carlo Probabilistic Inference for Learning COntrol
Link to MC-PILCO package (freely available from MERL research software):
- [https://www.merl.com/research/license/MC-PILCO](https://www.merl.com/research/license/MC-PILCO)

This package implements a Model-based Reinforcement Learning algorithm called Monte Carlo Probabilistic Inference for Learning and COntrol (MC-PILCO), for modeling and control of dynamical system. The algorithm relies on Gaussian Processes (GPs) to model the system dynamics and on a Monte Carlo approach to estimate the policy gradient during optimization. The Monte Carlo approach is shown to be effective for policy optimization thanks to a proper cost function shaping and use of dropout. The possibility of using a Monte Carlo approach allows a more flexible framework for Gaussian Process Regression that leads to more structured and more data efficient kernels. The algorithm is also extended to work for Partially Measurable Systems and takes the name of MC-PILCO-4PMS. Please see the related publication for a detailed description of the algorithm. The code is implemented in python3 and reproduces all the simulation examples in the related publication, namely, multiple ablation studies and the solution of a cart-pole system swing-up (available both in a python simulated environment and in the physic engine MuJoCo) and a trajectory controller for a UR5 (implemented in Mujoco). The results can be reproduced with statistical value via Monte Carlo simulations. The user has the possibility to add his own python system or Mujoco Environment and solve it with MC-PILCO or MC-PILCO-4PMS. Please refer to the guide for a more detailed explanation of the code base.


## Citation
If you use this MC-PILCO for any academic work, please cite our original [paper](https://arxiv.org/pdf/2101.12115.pdf).

```bibtex
@article{amadio2022mcpilco,
  author={Amadio, Fabio and Dalla Libera, Alberto and Antonello, Riccardo and Nikovski, Daniel and Carli, Ruggero and Romeres, Diego},
  journal={IEEE Transactions on Robotics},
  title={Model-Based Policy Search Using Monte Carlo Gradient Estimation With Real Systems Application},
  year={2022},
  volume={},
  number={},
  pages={1-20},
  doi={10.1109/TRO.2022.3184837}
}
```
