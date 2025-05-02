---
title: ✅ Varitional Auto Encoder!
summary: Basic concepts and foundations!
date: 2025-04-09
authors:
  - admin
image:
  caption: 'VAE General Architecture'
---
Varitional Auto Encoder(VAE!) is kind of single latent variable generative models which has the form Of P(X, Z), (do not judge a book from its cover if you find this joint probability ugly! 😛) where the X is the data point and Z is the latent Variable.
## Concepts
In VAE, you have two types of distributions, q(Z|X) and P(X|Z), each of them responsible for a specific task!
Actually, from the information theory, when you want to send the data over the internet, it is a very good idea to compress the data and then send it to your partner 😅 So your original data is X, and the Z is compressed data! And you have q(Z|X) distribution, and on your partner's side, they get the compressed data and should be required to decompress it, and the partner has P(X|Z) distribution.

## foundations
The Goal is to create a compressed sample z ~ q(Z|X) with the initial original data x, then send z to the Partner and try to recreate x ~ P(X|Z). til here! This architecture is called an Auto Encoder! (So you've learned Auto Encoder As well, am I a genius?😝), But wait a second, dude :) Where is the process of the new data point generation? Here, the god of probability enters :) What if we learn the q(Z|X) distribution? We can create a meaningful Z latent variable by getting a sample from the q(Z|X) distribution, which mimics the compressed version of data points, and passing it to the decoder P(X|Z), where it creates new data points that also mimic the original data points' patterns. So the final goal is to learn this variational Encoder and Decoder process!.

## Mathematics of VAE
The form of this generative model is P(X, Z) = P(X|Z). P(Z). The P(Z) is our prior, which can be considered as a Gaussian distribution, and P(X|Z) is our decoder or generative model, which needs Z to create a data sample X, see? We can recreate the input data sample X, or we can generate a new data sample X (this is a very important property, so pay attention to it :) ) this depends on latent code Z!, so if you pass the compressed version of X, which is Z here, you recreate the X or if you get sample Z from q(Z|X) ditributaion you can generate new data sample X which mimics the dataset patterns!. Til here we have our generative model, which is P(X, Z), but this generative model also needs Z! From here, I will talk about Z. 
Okay, by using the Bayesian formula, the q(Z|X) = q(X|Z).q(Z) / q(X), q(Z|X) is called posterior and q(Z) is called prior and q(X|Z) is our likelihood. Unfortunately, by the law of total probability, the q(X) is intractable! So we can not use this formula directly. Here we should approximate the posterior, which can be done using variational inference!

## Variational inference
Will be Continued....

