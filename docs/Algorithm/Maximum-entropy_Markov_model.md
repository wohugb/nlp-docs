# 最大熵马尔可夫模型 MEMM（Maximum-entropy Markov model）

最大熵模型的一个问题就是把每个字的标注问题分裂来看了，于是就有聪明人把马尔可夫链和最大熵结合，搞出了最大熵马尔可夫模型，这样不仅可以利用最大熵的各种 feature 的特性，而且加入了序列化的信息，使得能够从整个序列最大化的角度来处理，而不是单独的处理每个字，于是 MEMM 是求这样的形式

argmaxΠP(ci∣∣ci−1,ai)