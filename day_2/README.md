# Content
lecture material for the second day -- generative AI

In the folder slides you find the pdf of the lecture slides and the folder notebooks contains jupyter notebooks for the tutorials.

## Tutorials

### notebooks/Autoencoder.ipynb  
This notebook serves a the startig point to explore a plain autoencoder.
This notebook reproduces the two moons dataset with an auoencoder and shows how this already creates some problems. Furthermore, a convolutional autoencoder is applied on the MNIST dataset. The 2D latent space is visualised for each label, showing the irregularities of the autoencoder latent space. When trying to generate data, some problems occur, which are then treated in the next notebook.

### notebooks/VariationalAutoencoder.ipynb
Here, the same datasets are used as above. Only the autoencoder is expanded to a VAE. The trade-off of reconstuction and generation can be observed in both datasets. The gaps in the latent space of the autoencoder are not appearing for the VAE, creating higher quality synthetic data. 