---
title: ✅ Varitional Auto Encoder!
summary: Basic concepts and foundations!
date: 2025-04-09
authors:
  - admin
image:
  caption: 'VAE General Architecture'
---
Varitional Auto Encoder(VAE!) is kind of single latent variable generative model which has the form of P(X,Z), (do not judge a book from its cover if you find this joint probability ugly! 😛) and the X is the data point and zi is the latent Variable.
## Concepts
In VAE you have two type of distribution q(Z|X) and P(X|Z) each of them responsible for specific task!
Actually from the information theory when you want to send the data over internets, its very good idea to compress the data and then send it to your partner 😅 So your orginal data is X and the Z is compress data! and you have q(Z|X) distribution and in your partner side, they get the compress data and should require to decompress it, and the partner has P(X|Z) distribution.
