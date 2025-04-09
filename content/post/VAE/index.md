---
title: ✅ Varitional Auto Encoder!
summary: Basic concepts and foundations!
date: 2025-04-09
authors:
  - admin
image:
  caption: 'VAE General Architecture'
---
Varitional Auto Encoder(VAE!) is kind of single latent variable generative model which has the form of P(X,Z), (do not judge a book from its cover if you find this joint probability ugly! 😛) where the X is the data point and zi is the latent Variable.
## Concepts
In VAE you have two type of distribution q(Z|X) and P(X|Z) each of them responsible for specific task!
Actually from the information theory when you want to send the data over internets, its very good idea to compress the data and then send it to your partner 😅 So your orginal data is X and the Z is compress data! and you have q(Z|X) distribution and in your partner side, they get the compress data and should require to decompress it, and the partner has P(X|Z) distribution.

## foundations
The Goal is to create compress sample z ~ q(Z|X) with initial orginal data x, then send z to Partner and try to recreate x ~ P(X|Z). til here! this arcitecture Called Auto Encoder! (So you've learned Auto Encoder As well, am i genius?😝), where is the process of new data point generation? here the god of the probability enters :) what if we learn the q(Z|X) distribution? in which we are able to create meaningful Z latent varible which mimics the compress version of data points and then by sampling from q distribution, and passing to decoder (P(X|Z)) and it creates new data points which also mimics the orginal data points patterns. So the goal is to learn this Encoder Decoder process!.

## Mathematics of VAE
So we want to learn q(Z|X) right? lets assume that q has the form of normal distribution, q(Z|X) = N(Z|&mu;,&sigma;)
by using a nerual network in the form of e(x) = (&mu;&sigma;) and predicting &mu; and &sigma; we can create the q(Z|X) = N(Z|&mu;,&sigma;) = 1 / (σ√(2π)) * e^(-(x−μ))² / 2σ²

