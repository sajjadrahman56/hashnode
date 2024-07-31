---
title: "Gemini API :  Part 01"
seoTitle: "Introduction to Gemini API"
seoDescription: "Learn about Google's Gemini API and understand the fundamentals of Large Language Models (LLMs) and their applications"
datePublished: Tue Jul 30 2024 19:45:25 GMT+0000 (Coordinated Universal Time)
cuid: clz8tvada000209l53ia9hxl7
slug: gemini-api-part-01
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1722447640953/67d90222-f744-41a9-8b4b-fe6ee7ed4972.jpeg
tags: ai, google, deep-learning, transformers, llm, generative-ai, large-language-models, sajjadrahman, gemini

---

We live in an era of state-of-the-art LLMs (Large Language Models), where new models emerge almost daily. Gemini is one such LLM developed by Google.

Before using the Gemini API, it's essential to have a clear understanding of LLMs, as this knowledge can help in various tasks like fine-tuning models.

### What is LLM?

A Large Language Model (LLM) is a specialized machine learning model that can generate text from a prompt and perform language translation. It predicts the next word based on probabilities derived from a massive sequence of words. The transformer architecture is at the core of most LLMs.

In 2017, Google's research team introduced the transformer model in a research paper titled "Attention is All You Need." Due to its efficiency, scalability, and superior performance, the transformer model stands out from traditional machine or deep learning models.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1722446938564/d4e163f0-f0f6-41a4-a04f-b13148e4c622.png align="center")

Many people mistakenly think that `LLMs` are only used for chat applications. However, they have numerous applications, such as being used in virtual home devices like Amazon Alexa.

### Can we run LLM on the end device?

Running an LLM model on-premises is difficult due to computational costs and potential overload errors. For these reasons, many LLMs are accessible through a web interface or an API. The user's request, in text form, is sent to the pre-trained model via the API.

Gemini, or Gemma models, are a series of state-of-the-art language models developed by AI researchers at Google. The Gemini series includes Ultra, Pro, Flash, and Nano models, each designed for specific tasks. All of these models are accessible through the Google Gemini API.

### How Probabilistic Works ?

In natural language processing, predicting the next word in a sentence is often influenced by probabilities assigned to each word in the vocabulary. For instance, consider the partial sentence

`"I eat - - -."`

The model needs to choose a word to complete this sentence. Given a set of possible words like cat(0.02), dog(0.002),mango(0.88), and apple (0.6), each word has an associated probability that indicates how likely it is to follow the given context.

In this example, "mango" has a probability of 0.88, while "apple" has a probability of 0.6. Since "mango" has the highest probability, the model selects it as the most likely word, completing the sentence as "I eat mango."

Although "apple" is also a reasonable choice, the model prioritizes the word with the highest probability. This approach illustrates how large language models (LLMs) choose the next word based on probability values, ensuring the most contextually appropriate word is selected.

We will explore the transformer architecture in the next section.