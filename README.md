# Horovod
<p align="center"> 
<img src="images/IBM.png" width="450px" height="200px">
 </p>

<p align="center"><img src="https://user-images.githubusercontent.com/16640218/34506318-84d0c06c-efe0-11e7-8831-0425772ed8f2.png" alt="Logo" width="200"/></p>

[Horovod](https://github.com/uber/horovod) is a distributed training framework for TensorFlow, Keras, and PyTorch. The goal of Horovod is to make
distributed Deep Learning fast and easy to use. The following guide is an example showing how to use Horovod to quickly train a neural network.

# Table of Contents 
1. [Sign up for an IBM Cloud account](#signup)
2. [Provision an instance of Watson Studio and IBM Cloud Object storage](#provision)
3. [Add data to IBM Cloud Object Storage](#adddata)
4. [Create model with Horovod](#create)
5. [Train model with Horovod](#train)
5. [Results](#results)

## Sign up for an IBM Cloud account  <a name="signup"></a>
Registration for IBM Cloud can be done [here](https://console.bluemix.net/registration/?)

## Provision IBM Cloud Services  <a name="provision"></a>
Two services will be need to use Horovod on IBM Cloud: Watson Studio and IBM Cloud Object Storage. Watson Studio . IBM Cloud Object Storage stores training data and neural network model defintions. Watson Studio's Deep Learning service allows data scientists to train large scale neural network models on GPU-clusters, and deploy and manage them as API endpoints. Horovod allows data scientist to train neural network models on multiple GPU's in parallel, this capability *is not* allowed with a Watson Studio Lite account, therefore either a Standard V1 or Enterprise V2 account is needed.


