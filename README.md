# DCGAN架構生成cifar10中鹿的圖像
與GAN不同之處在於，Generator、Discriminator的架構從原本的fully connected layer改為捲積連結層(CNN)
## Archeitecture
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/DCGAN.png)
```
Note:此架構之shape為示意圖，與本project不同
```
## Difference between GAN and DCGAN
* GAN中的Generator、Discriminator使用的是fully connected layer，而DCGAN是在GAN原本的架構下將網路結構改為CNN
* Genrator、Discriminator 中每層皆使用 Batch Normalization 加快運算速度(其中Discrimator的第一層不必使用)
* Genrator、Discriminator 皆不使用 pooling 層 而是使用轉置卷積層（transposed convolutional layer）進行取樣
* Genrator 的每層皆用leaky Relu，最後一層使用tanh
* Discriminator的每層皆用leaky Relu，最後一層使用sigmoid
## Result
![error](https://github.com/JusticeLeee/DC_GAN/blob/master/deer.png)
## 加載說明
若加載github中的ipynb文件失敗，可直接透過[此連結查閱](https://nbviewer.jupyter.org/github/JusticeLeee/DC_GAN/blob/master/DcGan_deer.ipynb)

