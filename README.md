# node-feature-supported-LightGCN-for-movie-recommendation


This is more like a tutorial than a project. 

LightGCN is a graph neuronetwork model that can be used for recommendation or link prediction. Before starting the notebook, I recommend to read the paper *LightGCN: Simplifying and Powering Graph Convolution Network for Recommendation*(https://arxiv.org/abs/2002.02126). LightGCN is designed for faster training by excluding feature transformation and nonlinear activation.

However, we can still include some node features in LightGCN to compare the performance with standard LightGCN, and perhaps to trade-off between model complexity and prediction accuracy. So here I developed a customized LightGCN model to include node features. 

Notice that in torch_geometric, we alredy have built in lightGCN model (https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.LightGCN.html?highlight=lightgcn). I also recommed to check the source code in torch_geometric.nn.models.lightgcn for a better understanding so you can follow smoothly with this notebook as most part of my customized model are pretty similar to the torch_geometric.nn.models.lightgcn.
