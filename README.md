# **GPT Model from Scratch**

<p align="center">
  <img src="https://cdn.prod.website-files.com/649d5f7142f0800f8b55fbaa/64b57a26c8883a951510224e_641351aeefc0453800d820ec_co.gif" width="500" style="border-radius: 15px;" />
</p>

This repository shows how to build a **tiny** character-level GPT model *from scratch* using PyTorch. The model is trained on the classic text of **Don Quijote** from [Project Gutenberg](https://www.gutenberg.org/ebooks/2000).

## **What’s Inside**
- **Data Preparation**  
  Basic steps to download and encode *Don Quijote* at the character level.
  
- **Transformer Architecture**  
  - **Self-Attention** and **Multi-Head Attention**  
  - **Positional Embeddings**  
  - **Feedforward Layers**  
  - **Layer Normalization**  
  - **Causal Masking** (so the model can’t peek ahead)
  
- **End-to-End Notebook**  
  A single notebook that:
  1. Loads the data.  
  2. Defines a GPT-style Transformer in pure PyTorch.  
  3. Trains the model using a simple training loop.  
  4. Generates new text from the trained model.  
  5. Visualizes **attention maps** to illustrate how tokens attend to one another.

## **Attention Visualization**

One highlight of this project is the ability to see *where* the model focuses at each decoding step. We plot attention heatmaps for each head in every layer, giving you insight into how GPT-like models track context and build meaning:

<p align="center">
  <img src="attention_visualization.gif" width="400" />
</p>


## **References**
- [**Attention Is All You Need**](https://arxiv.org/abs/1706.03762) — Vaswani et al. (2017)  
- [**GPT-2 & GPT-3**](https://openai.com/research) by OpenAI  
- [**Project Gutenberg**](https://www.gutenberg.org/ebooks/2000) for *Don Quijote* text  
- [**The Illustrated Transformer**](http://jalammar.github.io/illustrated-transformer/) by Jay Alammar  

---
