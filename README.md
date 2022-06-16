## Reproducing GCN Paper

This repo reproduces the SGC paper [2] and compares the running time of the model and the running time of the original GCN.:

#### Files
- `README.md`: This file
- `train.py`: The main file for training and measuring training time for both models
- `model.py`: The model definition (GCN and SGC)
- `utils.py`: Utility functions
- `data`: Citation networks (Cora, CiteSeer, Pubmed)

#### How to run

```bash
    python train.py --data data/cora --epochs 100 --lr 0.01 --weight_decay 0.0005
```
be aware the hyperparameters are tuned for the sgc model not gcn.


#### Reference
```
@misc{https://doi.org/10.48550/arxiv.1609.02907,
  doi = {10.48550/ARXIV.1609.02907},
  url = {https://arxiv.org/abs/1609.02907},
  author = {Kipf, Thomas N. and Welling, Max},
  keywords = {Machine Learning (cs.LG), Machine Learning (stat.ML), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {Semi-Supervised Classification with Graph Convolutional Networks},
  publisher = {arXiv},
  year = {2016}, 
  copyright = {arXiv.org perpetual, non-exclusive license}
}

@misc{https://doi.org/10.48550/arxiv.1902.07153,
  doi = {10.48550/ARXIV.1902.07153},
  url = {https://arxiv.org/abs/1902.07153},
  author = {Wu, Felix and Zhang, Tianyi and Souza, Amauri Holanda de and Fifty, Christopher and Yu, Tao and Weinberger, Kilian Q.},
  keywords = {Machine Learning (cs.LG), Machine Learning (stat.ML), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {Simplifying Graph Convolutional Networks},
  publisher = {arXiv},
  year = {2019},
  copyright = {arXiv.org perpetual, non-exclusive license}
}
```

#### TODO
- [ ] Add training curve
- [ ] Add animations to the training
- [ ] Add visualization of the embedding
