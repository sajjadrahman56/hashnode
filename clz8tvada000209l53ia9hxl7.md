---
title: "All about Gemini API :  Part 01"
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

### How Probabilistic Works?

In natural language processing, predicting the next word in a sentence is often influenced by probabilities assigned to each word in the vocabulary. For instance, consider the partial sentence

`"I eat - - -."`

The model needs to choose a word to complete this sentence. Given a set of possible words like cat(0.02), dog(0.002), mango(0.88), and apple (0.6), each word has an associated probability that indicates how likely it is to follow the given context.

In this example, "mango" has a probability of 0.88, while "apple" has a probability of 0.6. Since "mango" has the highest probability, the model selects it as the most likely word, completing the sentence as "I eat mango."

Although "apple" is also a reasonable choice, the model prioritizes the word with the highest probability. This approach illustrates how large language models (LLMs) choose the next word based on probability values, ensuring the most contextually appropriate word is selected.

We will explore the transformer architecture in the next section.

Let's Explore some variations of Gemini model variations

#### Model Varitent

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1725112240215/0c92b4ee-dcfb-40e9-afd7-3e98c38db8af.png align="center")

These models are available on the #Gemini family. This picture is collected from the official Gemini documentation page. For more updates look [here](https://ai.google.dev/gemini-api/docs/models/gemini) .

We see here the Gemini 1.5 Flash, 1.5 Pro, and 1.0 Pro! Why these versions?

We have the idea that different machine learning algorithms are designed to solve different types of problems. According to the problem, we select the best model. Similarly, Gemini is now the state-of-the-art model from Google, which solves various problems and is used everywhere, including search bars, email writing, and summarizing.

If we look the simple comparison between `1.5 flash` and `1.5 pro`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1725112711101/c59acd71-5b24-4f38-beab-e09abdddcb08.png align="center")

We see here that `flash` is cost-effective compared to the `1.5 pro` model. On the other hand, both models take multimedia input ( audio, image, text, and video). When we consider the performance rather than the cost we must select the Gemini 1.5 Pro over the Gemini 1.5 Flash.