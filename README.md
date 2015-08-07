# VGGNets for Scene Recognition

Here we release our trained VGGNet models on the large-scale Places205 dataset, called **Places205-VGGNet** models, from the following reports:

    Places205-VGGNet Models for Scene Recognition
    Limin Wang, Sheng Guo, Weilin Huang, and Yu Qiao, in arXive, 2015

#### Performance on the Places205 dataset

<table>
    <tr>
        <td></td> <td>top-1 val/test</td>  <td>top-5 val/test</td>
        
    </tr>
    <tr>
        <td>Places205-VGGNet-11</td> <td>58.6/59.0 </td> <td>87.6/87.6</td>
    </tr>
     <tr>
        <td>Places205-VGGNet-11</td> <td>60.2/60.1</td> <td>88.1/88.5</td>
    </tr>
    <tr>
        <td>Places205-VGGNet-11</td> <td>60.6/60.3</td> <td>88.5/88.8</td>
    </tr>
</table>

#### Performance on the MIT67 and SUN397 dataset

<table>
    <tr>
        <td></td> <td>MIT67</td>  <td>SUN397</td>
    </tr>
    <tr>
        <td>Places205-VGGNet-11</td> <td>82.0 </td> <td>65.3</td>
    </tr>
     <tr>
        <td>Places205-VGGNet-11</td> <td>81.9</td> <td>66.7</td>
    </tr>
    <tr>
        <td>Places205-VGGNet-11</td> <td>81.2</td> <td>66.9</td>
    </tr>
</table>

#### Downloading
coming soon

#### Multi-GPU Implementation

In order to speed up the training procedure of VGGNets, we use a Multi-GPU extension of Caffe toolbox:

https://github.com/yjxiong/caffe/tree/action_recog

Meanwhile, we add the strategies of multi-scale cropping and corner cropping provided by this extension, which has been proved to be effective for action recognition in videos.
