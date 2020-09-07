# Using DCGAN generate deer picture in cifar10
```
Both Genrator and discriminator use leaky Relu.
However,generator's final layer use tanh,and discriminator's is sigmoid.
```
### Environment
* Jupyter Notebook
* Python 3.6
* Tensorflow 1.9-GPU
## Archeitecture
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/DCGAN.png)
```
Note:此架構之shape為示意圖，與本project不同
```

## DCGAN's advantages compare to GAN
* In GAN model, both generator and discriminator use Fully Connected Layer, but DCGAN use Convolution Neural Network.
* Both Genrator and Discriminator use Batch Normalization for speeding up calculation. ```(Note:Discrimator's first layer not use.)```
* Both Genrator and Discriminator not use pooling layer,but use transposed convolution layer.
## Result
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/deer.png)
## 加載說明
若透過網頁載入此ipynb文件失敗，可直接透過[此連結查閱](https://nbviewer.jupyter.org/github/JusticeLeee/DC_GAN/blob/master/DcGan_deer.ipynb)

