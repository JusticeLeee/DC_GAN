# Using DCGAN generator deer picture in cifar10
Both Genrator use leaky Relu, generator's final layer use tanh,and discriminator's is sigmoid.## Archeitecture
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/DCGAN.png)
```
Note:此架構之shape為示意圖，與本project不同
```
## Difference between DCGAN and GAN
* In GAN model, both generator and discriminator use Fully Connected Layer, but DCGAN using Convolution Neural Network.
* IN DCGAN, both Genrator and Discriminator use Batch Normalization for speeding up calculation.(Note:Discrimator's first layer not use.)
* IN DCGAN, both Genrator and Discriminator not use pooling layer,but using transposed convolution layer.
* Both Genrator use leaky Relu, generator's final layer use tanh,and discriminator's is sigmoid.
## Result
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/deer.png)
## 加載說明
若加載github中的ipynb文件失敗，可直接透過[此連結查閱](https://nbviewer.jupyter.org/github/JusticeLeee/DC_GAN/blob/master/DcGan_deer.ipynb)

