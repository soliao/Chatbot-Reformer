# Chatbot-Reformer


Building a chatbot using the Reformer model by Trax


Last updated: 04/01/2021

Todo next:

- Build a chatbot using PyTorch


---
## Project Summary

1. This project built a chatbot by using the Reformer architecture and trained on the MultiWOZ dataset from scratch.

2. After training on the MultiWOZ dataset for 20,000 epochs, the model achieved the **accuracy of 67.15%** on the test set (training/test size = 9938/500).

3. The chatbot learned to have a conversation with the custumer for helps on purchasing train tickets, booking a restaurant, giving directions, etc.

4. By feeding in some custom stencences, the **chatbot is able to handle the conversation and address the request**.

---

## References

This notebook was learned and modified from the assignment of the course [Natural Language Processing with Attention Models](https://www.coursera.org/learn/attention-models-in-nlp) on *Coursera* with the following amendments:

1. Instead of using a pre-trained model, I trained the chatbot **from scratch**

2. Instead of using `trax.supervised.decoding.autoregressive_sample_stream`, I used a helper function to continue the conversation token by token.

3. I cleaned up and rewrited the part of model evaluation. The model can be used to predict on the test dataset, or any custom starter sentence.

---

## The Reformer

N. Kitaev et al., **Reformer: The Efficient Transformer**

https://arxiv.org/abs/2001.04451
