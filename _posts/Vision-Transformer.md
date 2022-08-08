



# The Pros and Cons of CNNs

**Pros**:
CNN has inductive biases like translation invariance and locally restricted receptive field. Translational invariance recognizes an object even when its appearance varies, like changing orientation or zoom in or zoom out.

**Cons**:
Specifically designed for images.
It has a domain-specific design and is not scalable for it to be domain agnostic. CNN uses pixel arrays where each pixel represents varying importance and is domain-specific.
CNN lacks a global understanding of the images. It only looks for the presence of the image's features and does not understand the structural dependency between its features.
Computationally expensive: each pixel bears varying importance for the target task, which causes redundancy in both computation and representations.


# What is Vision Transformer?
Transformers have great success with NLP and are now applied to images. CNN uses pixel arrays, whereas Visual Transformer(ViT) divides the image into visual tokens.


1. Split an image into patches (fixed sizes)
2. Flatten the image patches
3. Create lower-dimensional linear embeddings from these flattened image patches
4. Include positional embeddings
5. Feed the sequence as an input to a state-of-the-art transformer encoder
6. Pre-train the ViT model with image labels, which is then fully supervised on a big dataset
7. Fine-tune the downstream dataset for image classification


https://uvadlc-notebooks.readthedocs.io/en/latest/tutorial_notebooks/tutorial15/Vision_Transformer.html
