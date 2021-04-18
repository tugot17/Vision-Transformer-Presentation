# NF-Nets-Presentation


[![Website perso.crans.org](https://img.shields.io/website-up-down-green-red/http/perso.crans.org.svg)](https://tugot17.github.io/Vision-Transformer-Presentation)
[![](https://images.microbadger.com/badges/license/nbrown/revealjs.svg)](LICENSE)

Presentation on Visual Transformer conducted at Wrocław University of Science and Technology on 21 April. 2021.

We discuss findings presented in [An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale](https://arxiv.org/abs/2010.11929) by Dosovitskiy, et al. and some earlier works. We introduce the concept of Vision Transformer, evaluate its advantages and disadvantages and make a few predictions on the future of the domain. 

Presentation available at: [tugot17.github.io/Vision-Transformer-Presentation](https://tugot17.github.io/Vision-Transformer-Presentation)

<img src="assets/vit.gif" width="500px"></img>

Gif by: [lucidrains](https://github.com/lucidrains/vit-pytorch)

## Video Summary



## TL;DR

In October 2020 Dosovitskiy et al. proposed a new computer vision architecture - Vision Transformer.
Even though it is used for computer vision tasks, it has no convolutional layers.
Authors show that it is possible to build a SOTA model using a pure transformer approach - something that until now was not possible.

To avoid the quadratic complexity issue present in transformers, authors divide input images into small patches of local pixels.
This plays a similar role to input embedding in NLP problems. Later that embedding is fed into the transformer-encoder 
layer and
the output of this operation is used for image classification.

The obtained results are very impressive. Using the transformer-only architecture it was possible to outperform the much bigger CNN models when given enough data. However, the same effect was not present when trained on smaller datasets (e.g ImageNet).
It suggests, that similarly to the situation present in NLP problems, transformers require much bigger amounts of data to
perform well, but when given they achieve outstanding results.

The publication of a pure transformer architecture that is capable of surpassing CNN may announce a paradigm shift in the design of computer vision models. The number of publications already extends the concept presented by Dosovitski et al. and achieves SOTA results in tasks traditionally solved with CNNs. The demand for large chunks of data can further widen the gap between large laboratories and independent researchers in terms of the results they achieve and
might shape the future of the domain.

## Author

- [Piotr Mazurek](https://github.com/tugot17)
