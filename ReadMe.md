# To implement deep learning algorithm in option pricing and compare the result with Black Scholes formula for calculating options.

## Option Price Basics:

1. Options are high risky derivatives that give option buyers the right to buy/sell a
   security at price on or before maturity.
2. Price of options is also called premiums which consist of sum of its intrinsic and
   extrinsic value.
3. **Intrinsic value** is the amount of money received immediately if an option were
   exercised less than strike price.
4. **Extrinsic value** is remaining value which exceeds the intrinsic value in premiums

## Step for parameter and training model:-

1. **Creating Dataset** - We randomly generated data of **300,000** option calls.
2. **Training Set** - Comprises of **2,40,000** call prices.
3. **Validation set** - **60,000** prices.
4. Pricing function is linearly normalized **i.e,C(S, K)/K = C(S/K, 1)**
5. Finally the normalized data is fit into deep net. 

## Details of Deep neural network

1. The size of input is **6 parameters**
2. Passed with **4 hidden layers** consisting of **100 neurons** each.
3. At each layer we have used different Activation function according to the inputs that are
    - **ELU**
    - **ReLU**
    - **LeakyReLU**

4. The loss function used is **MSE**
5. Epoch = 30
6. Batch size = 100

## These are the basics for learning Neural network for Financial models. There are many models Black-Scholes is one
