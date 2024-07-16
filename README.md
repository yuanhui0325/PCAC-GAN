#  PCAC-GAN:ASparse-Tensor-Based Generative Adversarial Network for 3D Point Cloud Attribute Compression

PCAC-GAN/
│
├── data/
│   ├── your_point_cloud_data.ply
│
├── checkpoints/
│   ├── model1.pth
│   ├── model2.pth
│
├── main.py
├── module.py
├── nn.py
├── pc_error.py
├── test.py
├── trainer.py
├── config.yml
├── data_loader.py
├── entropy_model.py


## Requirments
cuda 11.8

pytorch 1.8

MinkowskiEngine 0.5 or higher

torchac 0.9.3

python 3.8

We recommend you to follow https://github.com/NVIDIA/MinkowskiEngine to setup the environment for sparse convolution. 


## Pre-trained models
We trained seven models with seven different parameters.
https://pan.baidu.com/s/1xfSJxzJ1yuPdFro2qfvi-w
code：wiwg 

## Usage

### Training
```shell
python trainer.py --batch_size 8 --learning 1e-4 --lamb 800 --dataset_path train_rootdir --val_path val_rootdir
```

### Testing

python test.py --dataset_path test_rootdir


