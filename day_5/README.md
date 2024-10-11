# Content
lecture material for the fith day -- Intro to ML for Astrophysics and differentiable Programming

## Differentiable Simulators

### [notebooks/simple_orbit.ipynb](https://github.com/TobiBu/graddays/blob/main/day_5/notebooks/simple_orbit.ipynb)
This notebook builds a very simple example of a "Schräger Wurf" using an explicit Euler scheme to integrate the orbit.
Then it moves on to reimplement a pure python code in Jax and calculating the gradient through the simulation.
Once that is done we will make use of autodiff to calculate the gradient through the simulation and perform gradient-based optimization of the gravitational constant. 


### [notebooks/simple_example.ipynb](https://github.com/TobiBu/graddays/blob/main/day_5/notebooks/simple_example.ipynb)
This notebook shows a more involved example of a 1d fluid code called [jf1uids](https://github.com/leo1200/jf1uids/tree/main?tab=readme-ov-file) by Leonard Storcks. It will walk you trhugh how to use the code to simulated a shock tube test.

### [notebooks/gradients_through_stellar_wind.ipynb](https://github.com/TobiBu/graddays/blob/main/day_5/notebooks/gradients_through_stellar_wind.ipynb)
This ntebook uses [jf1uids](https://github.com/leo1200/jf1uids/tree/main?tab=readme-ov-file) and autodiff to calculate the gradient through a stellar wind blown bubble simulation.

### [notebooks/wind_parameter_optimization.ipynb](https://github.com/TobiBu/graddays/blob/main/day_5/notebooks/wind_parameter_optimization.ipynb)
This ntebook uses [jf1uids](https://github.com/leo1200/jf1uids/tree/main?tab=readme-ov-file) and autodiff to find stellar wind parameters from the final fluid state via gradient-descent.

## More Advanced Tutorials

There is a really nice book on differentiable physics simulators called [Introduction to Differentiable Physics](https://physicsbaseddeeplearning.org/diffphys.html) by N. Thuerey, P. Holl, M. Mueller, P. Schnell, F. Trost, K. Um. This book provides extensive explanantions on differentiable physics simulators and how to make use of them. If you want to follow along some of the more advanced examples from the lectures, see their notebooks.

### [Optimizing Burgers Turbulence](https://colab.research.google.com/github/tum-pbs/pbdl-book/blob/main/diffphys-code-burgers.ipynb) 

### [Differentiable 2D fluid simualtions](https://colab.research.google.com/github/tum-pbs/pbdl-book/blob/main/diffphys-code-ns.ipynb) 

### [Reducing numerical errors with NNs](https://colab.research.google.com/github/tum-pbs/pbdl-book/blob/main/diffphys-code-sol.ipynb)

### [Solving inverse problems with NNs](https://colab.research.google.com/github/tum-pbs/pbdl-book/blob/main/diffphys-code-control.ipynb