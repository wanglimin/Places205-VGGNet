# VGGNets for Scene Recognition

Here we release our trained VGGNet models on the large-scale Places205 dataset, called **Places205-VGGNet** models, from the following report:

http://arxiv.org/abs/1508.01667

    Places205-VGGNet Models for Scene Recognition
    Limin Wang, Sheng Guo, Weilin Huang, and Yu Qiao, in arXive 1508.01667, 2015
    
#### Performance on the Places205 dataset

|        Model        | top-1 val/test | top-5 val/test |
|:-------------------:|:--------------:|:--------------:|
| Places205-VGGNet-11 |    58.6/59.0   |    87.6/87.6   |
| Places205-VGGNet-13 |    60.2/60.1   |    88.1/88.5   |
| Places205-VGGNet-16 |    60.6/60.3   |    88.5/88.8   |
| Places205-VGGNet-19 |    61.3/61.2   |    88.8/89.3   |


We use 5 crops and their horizontal flippings of each image for testing.

#### Performance on the MIT67 and SUN397 dataset

|        Model        | MIT67 | SUN397 |
|:-------------------:|:-----:|:------:|
| Places205-VGGNet-11 |  82.0 |  65.3  |
| Places205-VGGNet-13 |  81.9 |  66.7  |
| Places205-VGGNet-16 |  81.2 |  66.9  |

We extract the fc6-layer features of our trained Places205-VGGNet models, which are further normalized by L2-norm.

#### Download
- Places205-VGGNet-11: <br />
  http://mmlab.siat.ac.cn/Places205-VGGNet/siat_scene_vgg_11.caffemodel
- Places205-VGGNet-13: <br />
  http://mmlab.siat.ac.cn/Places205-VGGNet/siat_scene_vgg_13.caffemodel
- Places205-VGGNet-16: <br />
  http://mmlab.siat.ac.cn/Places205-VGGNet/siat_scene_vgg_16.caffemodel
- Mean file: <br />
  http://mmlab.siat.ac.cn/Places205-VGGNet/places205_mean.mat

These models are relased for non-conmercial use. If you use these models in your research, thanks to cite our above report.

#### Multi-GPU Implementation

In order to speed up the training procedure of VGGNets, we use a Multi-GPU extension of Caffe toolbox:

https://github.com/yjxiong/caffe/tree/action_recog

Meanwhile, we add the strategies of _multi-scale cropping_ and _corner cropping_ provided by this extension, which has been proved to be effective for action recognition in videos.

#### Questions
Contact 
- [Limin Wang](http://wanglimin.github.io/)
- [Sheng Guo] (mailto:sheng.guo@siat.ac.cn)
- [Weilin Huang](http://www.wlhuang.com/)

