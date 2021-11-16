# RRNet_TGRS2021

Runmin Cong, Yumo Zhang, Leyuan Fang, Jun Li, Chunjie Zhang, Yao Zhao, and Sam Kwong, RRNet: Relational reasoning network with parallel multi-scale attention for salient object detection in optical remote sensing images, IEEE Transactions on Geoscience and Remote Sensing, 2021.

Project: https://rmcong.github.io/proj_RRNet.html

## Code and Results of RRNet:

# RRNet
* Results:
  - We provide the resutls of our RRNet on EORSSD. 
```
Baidu Cloud: https://pan.baidu.com/s/1Zt6PsB5zAl4Tts_4g7I9OQ  Password: 1234
```
* Pretrained model:
  - We provide our testing code. If you test our model, please download the pretrained model, unzip it, and put the checkpoint `RRNet_pretrained.pth` to `Checkpoints/trained/` folder 
  and put the pretrained backbone `backbone_r.pth` to `Checkpoints/warehouse/` folder.
  - Pretrained model download:
```
Baidu Cloud: https://pan.baidu.com/s/1RtS4JQaW3f0RTq6o7h512g  Password: 1234
```

# Pytorch
* Pytorch implementation of RRNet

## Requirements

* Python 3.7
* Pytorch 1.5.1
* torchvision

## Data Preprocessing
* We resize the images of original EORSSD dataset. For your evaluations, we also provide the corresponding resized images and labels. 
If you test our model, please download the resized data, and put the data to `train_and_test/` folder.
* Resized EORSSD:
```
Baidu Cloud: https://pan.baidu.com/s/1CnbH_wSJBplo4UCMRInI3A  Password: 1234
```

## Test
```
python test.py
```

* You can find the results in the `'Outputs/Outputs_GR'` folder.
* You can use a script to resize the results back to the same size as the original RGB-D image,  or just use the results with a size of 224*224 for evaluations. 
We did not find much differences for the evaluation results.


## If you use our RRNet, please cite our paper:

    @article{RRNet,
       title={{RRNet}: Relational Reasoning Network with Parallel Multi-scale Attention for Salient Object Detection in Optical Remote Sensing Images},
       author={Cong, Runmin and Zhang, Yumo and Fang, Leyuan and Li, Jun and Zhang, Chunjie and Zhao, Yao and Kwong, Sam},
       journal={IEEE Transactions on Geoscience and Remote Sensing},
       year={2021},
       publisher={IEEE}
    }

## Contact Us:
If you have any questions, please contact Runmin Cong at rmcong@bjtu.edu.cn.
