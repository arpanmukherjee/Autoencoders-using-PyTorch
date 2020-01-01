
# Autoencoders using PyTorch

## Quick Links
- [About](#about)
- [Setup](#setup)
	- [Installation](#installation)
	- [Training](#training)
- [Results](#results)

## About
<p align="center">
	<img src="images/autoencoder.jpeg" height='400px'/><br>
	<code>Fig 1: Architecture of an Autoencoder</code>
</p>

## Setup
### Installation
1. Download the github repo by using following command running from terminal.
```
git clone https://github.com/arpanmukherjee/Autoencoders-and-more-using-PyTorch.git
cd Autoencoders-and-more-using-PyTorch/
```

2. Install `pip` from the terminal, for more details please look [here](https://pypi.org/project/pip/). Go to the following project folder and install all the dependencies by running the following command. By running this command, it will install all the dependencies you will require to run the project.
```
pip install -r requirements.txt
```

### Training
1. The network can be trained using `train.py` script. Currently it only accepts following arguments with the accpeted values. Please strictly follow the argument name name and any of the values.

| argument | accepted values | default value |
|--|--|--|
| data_path | data directory | ./dataset/ |
| dataset | MNIST or STL10 or CIFAR10 | - |
| epochs | integer | 75 |
| batch_size | integer | 28 |
| learning_rate | float | 0.001 |
| use_cuda | bool | - |
| network_type | FC or Conv | FC |

Arguments which has no default value, you must provide value to run the script.
```
python train.py --dataset STL10 --use_cuda True --network_type Conv
```
If you think model is taking too much time, you can consider using GPU. Set `use_cuda` argument as `True`.
## Results
