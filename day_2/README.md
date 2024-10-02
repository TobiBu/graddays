# Content
lecture material for the second day -- generative AI

In the folder slides you find the pdf of the lecture slides and the folder notebooks contains jupyter notebooks for the tutorials.

## VAE tutorials

### [notebooks/Autoencoder.ipynb](https://github.com/TobiBu/graddays/blob/main/day_2/notebooks/Autoencoder.ipynb)  
This notebook serves a the startig point to explore a plain autoencoder.
This notebook reproduces the two moons dataset with an auoencoder and shows how this already creates some problems. Furthermore, a convolutional autoencoder is applied on the MNIST dataset. The 2D latent space is visualised for each label, showing the irregularities of the autoencoder latent space. When trying to generate data, some problems occur, which are then treated in the next notebook.

### [notebooks/VariationalAutoencoder.ipynb](https://github.com/TobiBu/graddays/blob/main/day_2/notebooks/VariationalAutoencoder.ipynb)
Here, the same datasets are used as above. Only the autoencoder is expanded to a VAE. The trade-off of reconstuction and generation can be observed in both datasets. The gaps in the latent space of the autoencoder are not appearing for the VAE, creating higher quality synthetic data. 

### [notebooks/PlayingWithVAE.ipynb](https://github.com/TobiBu/graddays/blob/main/day_2/notebooks/PlayingWithVAE.ipynb)
Notebook by [Christian Kleiber](https://github.com/CKleiber/SciML-Seminar/tree/main) to play around with the concept of the VAE. It uses a comic face dataset to train a quite large VAE to test the interpolation and reconstruction of more complicated data than e.g. MNIST. It has some interactive features that will not work on colab and need to be executed with a local copy.

## Score matching tutorials

### [notebooks/ULA.ipynb](https://github.com/TobiBu/graddays/blob/main/day_2/notebooks/ULA.ipynb)  
This tutorial implements the unadjusted Langevin algorithm to sample from a SDE. 

### [notebooks/two_moons_demo.ipynb](https://github.com/TobiBu/graddays/blob/main/day_2/notebooks/two_moons_demo.ipynb)  
In this tutorial you will train a score model on the two moons dataset and learn how to sample from it.
Additionally, at the end there is a comparison to energy based models which we haven't covered in the lecture though.

This is a notebook originally written by Alexandre Adam from Montreal, Canada. It uses a package (score_models) available under his github account [here](https://github.com/AlexandreAdam/torch_score_models). If you end up using the code implementation presented here for any publication, please include citations to arXiv:2211.03812 [astro-ph.IM] and arXiv:2302.03046 [astro-ph.IM] (the last one for the SLIC implementation).

### [notebooks/score_based_modelling_overview.ipynb](https://github.com/TobiBu/graddays/blob/main/day_2/notebooks/score_based_modelling_overview.ipynb) 
In this tutorial you will follow a more in debth walk-through through the ideas and concepts behind score matching and Langevin dynamics. You will explore the effect of noise scheduling on approximation capabilities of the score model and learn how to sample using stochastic differential equations.

This is a notebook originally written by Alexandre Adam from Montreal, Canada. It uses a package (score_models) available under his github account [here](https://github.com/AlexandreAdam/torch_score_models). If you end up using the code implementation presented here for any publication, please include citations to arXiv:2211.03812 [astro-ph.IM] and arXiv:2302.03046 [astro-ph.IM] (the last one for the SLIC implementation).

### Additional notebooks
Additionally, there is some more advance notebooks available by Yang Song showing the potential of score mathcing models.
His awesome blog post can be found [here](https://yang-song.net/blog/2021/score/) and notebooks with example code in pytorch can be found [here](https://colab.research.google.com/drive/120kYYBOVa1i0TD85RjlEkFjaWDxSFUx3?usp=sharing) and the same notebooks in JAX [here](https://colab.research.google.com/drive/1SeXMpILhkJPjXUaesvzEhc3Ke6Zl_zxJ?usp=sharing). If you want to play around with more complex pre-trained models see [here](https://colab.research.google.com/drive/17lTrPLTt_0EDXa4hkbHmbAFQEkpRDZnh?usp=sharing) for pytroch models and [here](https://colab.research.google.com/drive/1dRR_0gNRmfLtPavX2APzUggBuXyjWW55?usp=sharing) for JAX versions. The entire code base coming with the blog post by Yang Song can be found [here](https://github.com/yang-song/score_sde_pytorch) for pytorch and [here](https://github.com/yang-song/score_sde) for JAX. 