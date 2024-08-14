# MDSGNN

Welcome to the source code repository for our paper: **Multi-order Spectral Graph Neural Networks: Fourier Expansion Meet Simplicial Complexes**


# Prerequisites:
Ensure you have the following libraries installed:
```
pytorch
pytorch-geometric
networkx
numpy
```



# Exp1: Node Classification 
go to folder `./node_classify/src`

## Run experiment with Citeseer:


```sh
cd node_classify/src
python run_node_exp.py    --dataset citeseer         --cuda 2   --net MDSGNN        --Order 2    --lr 0.005      --dropout 0.7  --weight_decay 5e-3  --alpha 0.5

```

Before the training commences, the script will download and preprocess the respective graph datasets. 
Subsequently, it performs the appropriate graph-lifting procedure (this process might a while).


# Exp2: graph classification
go to folder `./graph_classify`

We prepared individual scripts for each experiment. The results are written in the
`exp/results/` directory and are also displayed in the terminal once the training is
complete. 
```shell
cd graph_classify
sh scripts/MDSGNN-PROETINS.sh
```


 
Thank you for your interest in our work. If you have any questions or encounter any issues while using our code, please don't hesitate to raise an issue or reach out to us directly.


