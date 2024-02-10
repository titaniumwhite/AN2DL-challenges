# Deep Learning challenges #
### @Politecnico di Milano, Academic Year 2021-2022, Artificial Neural Network and Deep Learning course ###
The aim of the two challenges was to develop multiples models of neural network in order to solve specific problems. This first challenge aimed to classify images of leaves using Convolutional Neural Networks or Transfer Learning. Instead, in the second challenge we had to create a Neural Network to predict future samples of a multivariate series.
<br/><br/>

### Challenge1 - leaf challenge ###
Firstly, the dataset has been analysed. We applied data augmentation to enhance the model's ability to handle diverse leaf images. Additionally, class imbalance was addressed through ```class_weight``` from ```sklearn``` and the dataset was divided into training and validation sets. ```Keras TensorBoard callbacks``` were used to monitor and optimize the learning process. Among all the models, the one which gave best accuracy is model3 which makes use of Transfer Learning (VGG16) and Fine Tuning and a series of multiple Dropout and Dense Layers.   
<p align="center">
<img src=https://github.com/titaniumwhite/AN2DL-challenges/blob/main/images/model3cm.png width="50%" align="center">
</p>   
<p align="center">
<img src=https://github.com/titaniumwhite/AN2DL-challenges/blob/main/images/model3accuracy.png width="48%" align="left">
<img src=https://github.com/titaniumwhite/AN2DL-challenges/blob/main/images/model3loss.png width="48%" align="right">
</p>   
<br/><br/>
<br/><br/>
<br/><br/>
<br/><br/>

### Challenge2 - timeseries challenge ###
In the second challenge we had to create a Neural Network to predict future samples of a multivariate series. Once divided the dataset in train and validation, we
decided to use during the first training a window of 200 and a stride of 10. During the challenge, we fine-tuned these two parameters. The model which gave a best accuray is model4, composed by an LSTM of 64 units, a dropout layer, another LSTM of 128 units, one Global Average Pooling layer and another dropout. Both LSTMs had kernel regularized and recurrent regularizer.  

<p align="center">
<img src=https://github.com/titaniumwhite/AN2DL-challenges/blob/main/images/model4_mae.png width="48%" align="left">
<img src=https://github.com/titaniumwhite/AN2DL-challenges/blob/main/images/model4_rmse.png width="48%" align="right">
</p>   


