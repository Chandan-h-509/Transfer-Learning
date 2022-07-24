# Transfer-Learning
Transfer Learning in PyTorch

In this project I have implemented the concept of Transfer Learning.
I have used the pretrained ResNet18 model which is trained on the ImageNet dataset(containing 1.2 million images with 1000 categories.)
Using this pretrained model, I have trained a new model which classifies wheteher a particular image is "ANT" or a "BEE".

The techiques used are:
1. Finetuning the convnet: Here the last few layers are changed and the entire network is trained on the new data.
2. ConvNet as fixed feature extractor: Here, we will freeze the weights for all of the network except that of the final fully connected layer. This last fully connected layer is replaced with a new one with random weights and only this layer is trained.
