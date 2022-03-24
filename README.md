## Deep learning training framework from scratch

### 1. Framework design

In this project, we design a simple neural network from scratch with basic modules like Linear(fully connected
layers), Tanh, and ReLU and Sequential layers to combine several modules in basic sequential structure, loss
modules like MSE and BCE and optimizer modules like SGD and Adam. And then we test the framework
with a simple classification task.

The architecture shown as\
<img src="https://user-images.githubusercontent.com/58901415/160008828-844fb186-ddf7-4e5d-984a-4a31902fadcc.png" width="67%" height="67%" />

### 2. Experiments

Then the tests were done by importing the basic framework with sequential layers and generating a
training and a test set of 1000 points sampled uniformly in $[0, 1]^2$, each with a label 0 if outside the disk
centered at $(0.5, 0.5)$ of radius $1=\sqrt{2\pi}$, and 1 inside, build the basic network with two input units, two output
units, three hidden layers of 25 units, train the above network with MSE, logging the loss, compute and
prints the final train and the test errors. And then we test the performance of the basic network with Adam
optimizer.

The basic networks as\
<img src="https://user-images.githubusercontent.com/58901415/160010515-9a55c4a6-0a86-47c2-9c6d-50e2c28ce07d.png" width="32%" height="32%" />

### 3. Performances

Model parameters are initialized in uniform distribution randomly. We did 10 rounds and obtained curves of average loss and accuracy
per epoch of each round for each configuration of network. 

The classification results for test sets and training accuracy/loss as\
<img src="https://user-images.githubusercontent.com/58901415/160010886-660552f1-fc23-4f16-8266-4b6d205f0265.png" width="36%" height="36%" />\
The training accuracy/loss as\
<img src="https://user-images.githubusercontent.com/58901415/160011666-0f494dc9-dc58-4bb3-a9b5-b85b94c45638.png" width="72%" height="72%" />
<img src="https://user-images.githubusercontent.com/58901415/160011768-08241359-d8e0-4e53-899b-53c1508e6cd1.png" width="72%" height="72%" />
