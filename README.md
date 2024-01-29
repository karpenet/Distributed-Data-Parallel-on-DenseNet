# Distributed Data Parallel on DensNet

Distributed training using PyTorch on a DensNet Model.

### Requirements

* Python 3.8.6
```shell script
pip install -r requirements.txt
```

### Training

Single GPU training:
```shell script
CUDA_VISIBLE_DEVICES=0 python train.py
```

Distributed training using two GPUs:
```shell script
CUDA_VISIBLE_DEVICES=0,1 python train_ddp.py -g 2
```

Distributed training using two GPUs with Mixed Precision:
```shell script
CUDA_VISIBLE_DEVICES=0,1 python train_ddp_mp.py -g 2
```