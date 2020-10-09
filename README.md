# Using DCGAN model generate deer picture in cifar10
```
將大量的訓練資料透過捲積神經網路傳到全連接層後，經過訓練產生鹿的圖像
相較於傳統的深度學習網路，CNN除了全連接層之外，透過捲積層和池化層
來取得局部特徵及縮減圖片大小，達到大幅度提高訓練速度的效果
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
* Both Genrator and Discriminator use Batch Normalization for speeding up calculation. 
* Both Genrator and Discriminator different from traditional CNN ,they don't use pooling layer.
* Generator use tansposed convolution layer ,as known as deconvolution ,and Discrinator use convolution layer.
```
Note:Generator's final layer use tanh,and discriminator's is sigmoid.
```
## Result
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/deer.png)
## 加載說明
若透過網頁載入此ipynb文件失敗，可直接透過[此連結查閱](https://nbviewer.jupyter.org/github/JusticeLeee/DC_GAN/blob/master/DcGan_deer.ipynb)

