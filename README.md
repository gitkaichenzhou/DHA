
This repository contains the code for the framework in **DHA: End-to-End Joint Optimization of Data Augmentation Policy, Hyper-parameter and Architecture** (see [paper](https://arxiv.org/abs/2109.05765)).

## Downloads
### Dataset Preparation
Cifar10: https://www.cs.toronto.edu/~kriz/cifar.html
Cifar100: https://www.cs.toronto.edu/~kriz/cifar.html
IMAGENET: https://image-net.org/download.php
SPORTS8: http://vision.stanford.edu/lijiali/event_dataset/
MIT67: http://web.mit.edu/torralba/www/indoor.html
FLOWERS102: https://www.robots.ox.ac.uk/~vgg/data/flowers/102/


## Usage

### Training with flowers102 dataset

Training normal two-stage ISTA Model
```bash
python search_darts.py --conf_path conf/ista/flowers102_ista.json --Running ista_nor
```

Training normal single-stage ISTA Model
```bash
python search_darts.py --conf_path conf/ista/flowers102_ista_single.json --Running ista_single_nor
```

Training DHA Model
```bash
python search_darts.py --conf_path conf/ista/flowers102_ista_single.json --Running ista_single_doal
```
