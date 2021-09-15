---
layout: post
title: Statistical Learning Theory: An Overview
date: 2021-06-31 10:00:00
description: 
---



*[Machine Learning Techniques for Intrusion Detection in Network Security](https://epub.jku.at/obvulihs/content/titleinfo/4928712)*





Assume that we have $N$ independent and identically distributed (iid) labeled training observations 
\begin{equation}\label{equation:train-set}
    %\bm{Z}_N = 
    \mathcal{D}_N = \{(\bm{x}_n, y_n) \}_{n=1}^N
\end{equation}
where predictors $\bm{x}_n \in \mathcal{X} \subseteq \mathbb{R}^{D}$ are drawn % independently 
from an unknown probability distribution $P(\bm{x})$ and a binary target (label) variable $y_n \in \mathcal{Y}$ is drawn from unknown conditional distribution $P(y|\bm{x})$. Further assume that we have $M$ labeled iid testing observations
\begin{equation}\label{equation:test-set}
    %\bm{Z}_M = 
    \mathcal{D}_M = \{(\bm{x}_m, y_m) \}_{m=N+1}^{N+M}
\end{equation}
and assume that these samples are drawn from the same probability distributions as the set of training samples. The set of test samples will not be used for training of the model, but only for the final evaluation. 