# Using DCGAN model generate deer picture in cifar10
```
A large amount of training data is passed to the fully connected layer through the convolutional neural network and then trained to produce the image of the deer. Compared with the traditional deep learning network, in addition to the fully connected layer, it can pass through the convolutional layer and the pooling layer. Obtain local features and reduce the image size to greatly increase the training speed.
```
### Environment
* Jupyter Notebook
* Python 3.6
* Tensorflow 1.9-GPU
## Archeitecture
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/DCGAN.png)
```
Note:此架構之shape-size僅為示意圖，與本project不同
```

## DCGAN's advantages compare to GAN
* In GAN model, both generator and discriminator use Fully Connected Layer, but DCGAN use Convolution Neural Network archeitecture.
* Both Genrator and Discriminator use Batch Normalization for speeding up calculation. ```(Note:Discrimator's first layer not use.)```
* Both Genrator and Discriminator different from traditional CNN ,they don't use pooling layer.
* Generator use tansposed convolution layer ,as known as deconvolution ,and Discrinator use convolution layer.
```
Note:Generator's final layer use tanh,and discriminator's is sigmoid.
```
## Result
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/deer.png)
## 加載說明
若透過網頁載入此ipynb文件失敗，可直接透過[此連結查閱](https://nbviewer.jupyter.org/github/JusticeLeee/DC_GAN/blob/master/DcGan_deer.ipynb)

