# Scalable synthesis of new biomolecules using deep generative models
## Hayley Song

![motivation](/images/motivation.png)

# Related Works
- Deep generative models of genetic variation capture the effects of mutations. Nat Methods 15, 816–822 (2018). 
- Deep Sematic Protein Annotation Classification and Exploration
- A multiscale statistical mechanical framework integrates biophysical and genomic data to assemble cancer networks. Nat Genet 46, 1363–1371 (2014)
- Onto2vec: joint vector-based representation of biological entities and their ontology-based annotations. arXiv preprint arXiv:1802.00864.(2018)

# Embeddings
- Poincaré Embeddings for Learning Hierarchical Representations

# Dataset
- Protein Data Bank
- ProteinNet: a standardized data set for machine learning of protein structure
  - sequence and structure data
  - multiple sequence alignments (MSAs)

# Deep generative model: Poincaré-VAE (P-VAE)
## Challenges:
	- Learn meaningful (compressed) representation of protein molecules that preserve their hierarchical structures 
	- Learn to facilitate controllable generation of new, realistic proteins

## Deep generative models can solve to two challenges in one-go
	- Learn the mapping of an empirical distribution of observations to a lower dimensional Poincaré ball (Analysis/Abstrction/Compression)
	- Learn a map from the discovered latent space (aka. embedding space) to the observation space

## How?
	- Joint optimization of the encoder and the decoder networks 
	- Encoder is implemented as a deep neural network and is a stochastic function that maps the observed data to a latent representation
	- Decoder is also implemented as a deep neural network, and is a stochastic function that maps a latent vector (“code vector”) to a data realization (a possible/realistic/plausible protein molecule)
  
![vae1](/images/vae1.png)
---
## Related generative models
![gen-models](/images/gen-models.png)
![gen-mols](/images/gen-mols.gif)
---
![hyperbolic](/images/hyperbolic-space.png)
---
![desired-output](/images/desired-output.png)
---
![applications](/images/applications.png)
![learn](/images/learn.png)
![control](/images/control.png)

# Tools
- cuda: parallelized training of deep generative models
	- PyTorch
- VDM: interactive visualization of molecules




