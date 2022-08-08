
# What is Vision Transformer?
Transformers have great success with NLP and are now applied to images. CNN uses pixel arrays, whereas Visual Transformer(ViT) divides the image into visual tokens.


# The Pros and Cons of CNNs

**Pros**:
CNN has inductive biases like translation invariance and locally restricted receptive field. Translational invariance recognizes an object even when its appearance varies, like changing orientation or zoom in or zoom out.

**Cons**:
Specifically designed for images.
It has a domain-specific design and is not scalable for it to be domain agnostic. CNN uses pixel arrays where each pixel represents varying importance and is domain-specific.
CNN lacks a global understanding of the images. It only looks for the presence of the image's features and does not understand the structural dependency between its features.
Computationally expensive: each pixel bears varying importance for the target task, which causes redundancy in both computation and representations.
