# VisualizingNDF
The repository contains pre-trained model and code for visualizing deep neural decisoin forest.
(This repository is a beta version with more comments to write and more cleaning-up to do.) For now only classification models are released and you can contact me if you are interested in the regression models.

<div align="center">
    <img src="images/mnist_results.png">
</div>
<div align="center">
    <img src="images/cifar10_results.png">
</div>

## Requirements
* Python 3.6 (not tested for other versions)
* PyTorch 1.0 

## Pre-trained models
You can download the pre-trained models at https://drive.google.com/drive/folders/1DM6wVSknkYBqGf1UwHQgJNUp40sYDMrv?usp=sharing and place them in the "pre-trained" folder.

## Visualization
After downloading the pre-trained models,
simply run 
```bash
python ndf_vis.py 
```
for CIFAR-10.

For MNIST, run 
```bash
python ndf_vis.py -dataset 'mnist'
```
## Train
To train a neural decision forest for CIFAR-10, use 
```bash
python main.py
```
For MNIST, run 
```bash
python main.py -dataset 'mnist' -epochs 50
```
## Citation
Please cite the paper in your publications if it helps your research:

    @InProceedings{Li_2019_CVPR_Workshops,
    author = {Shichao Li and Kwang-Ting Cheng},
    title = {Visualizing the decision-making process in deep neural decision forest},
    booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
    month = {June},
    year = {2019}
    } 
    
Links to the paper:

- [Visualizing the decision-making process in deep neural decision forest](https://arxiv.org/abs/1904.09201)
