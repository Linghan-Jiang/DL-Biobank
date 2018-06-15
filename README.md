# Can deep learning improve genomic prediction of complex human traits?
This repo contains the code to reproduce the experiments of the paper [Can deep learning improve genomic prediction of complex human traits?](https://arxiv.org/...).


## Before you start

- Download and install [Tensorflow](https://www.tensorflow.org/install/) and [Keras](https://keras.io/#keras-the-python-deep-learning-library).
- Download the biobank dataset and traits.
- Run a GWAS for all traits and save the results in a file

## To run

#### Train MLPs models for height with 10k Best SNPS 
```python main.py --mlp --trait height```

#### Train CNNs models for height with 10k Unif SNPS 
```python main.py --cnn --trait height --unif```

#### Train MLPs models for BHMD with 50k Best SNPS 
```python main.py --mlp --trait BHMD --unif -k 50000```

#### Deep learning hyperparamer tuning 
- see GA directory

#### Figure 1 generation
- see Figure 1 notebook

## License
MIT
