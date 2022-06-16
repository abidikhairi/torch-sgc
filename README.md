## Reproducing GCN Paper

This repo reproduces the GCN paper [1] by using the following code:

#### Files
- `README.md`: This file
- `train.py`: The main file for training
- `model.py`: The model definition
- `utils.py`: Utility functions
- `data`: Citation networks (Cora, CiteSeer, Pubmed)

#### How to run

```bash
    python train.py --data data/cora --epochs 100 --lr 0.01 --weight_decay 0.0005
```

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
```

#### TODO
- [ ] Add training curve
- [ ] Add animations to the training
- [ ] Add visualization of the embedding
