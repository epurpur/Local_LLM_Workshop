```
-Last updated 06/21/24
```

# UVA Library Workshop on Running Large Language Models on your local computer

### Link to recording of this workshop



## About Me
* Erich Purpur: I am a Research Librarian for Science & Engineering in the Brown Science & Engineering Library. I've been at UVA since 2017.
* epurpur@virginia.edu

## Data Resources in the UVA Library
* [Research Data Services](https://data.library.virginia.edu/)
* [Workshop Series](https://data.library.virginia.edu/training/)

## Upcoming Workshops

| Workshop | Date | Time |
| ---- | ---- | ---- |
| Intro to Python pt 1                                                |       Tuesday 1/30   |  12:00 - 1:30pm


## Things to have before we begin


# Disclaimer
I am not an AI expert! We are all learning and navigating this confusing landscape together. 


# Background Information 
## Large Language Models
A Large Language Model (LLM) is an artificial intelligence system designed to understand and create human-like content across various media types including text, images, video, etc. These models are trained on extensive datasets of diverse information. Using deep learning techniques, they recognize patterns and relationships within and between different forms of media.

In simpler terms, an LLM is a computer program that has been fed enough examples of human language that it can recognize and interpret human language and other forms of complex data. Many LLMs are trained on data that has been gathered from the internet and the quality of the samples impacts how well the LLM will learn natural language. 

There are many LLMs in existence such as OpenAI's high profile GPT (Generative Pre-Trained Transformer). Some are optimized for specific purposes, as we will learn more about today, while others are more general use. 

LLMs are composed of large files that contain the parameters and architecture defining the model. These can be several gigabytes in size. Once the model is downloaded, it may need to be configured for a specific task. 


## Why?

You might be wondering, why would I want to run an LLM directly on my machine?

1. Privacy and Security

By processing information locally, Ollama ensures that your information remains secure and private. According to their [terms of service](https://openai.com/policies/terms-of-use/), OpenAI claims they are not keeping and misusing your data. However, there are concerns about that. UVA licenses [UVA CoPilot](https://virginia.service-now.com/its?id=itsweb_kb_article&sys_id=8a0050d847fac610bb2b9c7b116d4317), an instance of Microsoft CoPilot, which is probably safer to use. These concerns are negated if you run the LLM yourself!

2. Offline Use

At least with Ollama, if you have a scenario where the internet is not available, such as use in the field, you can still run your AI models because it is saved on your local machine. Similarly, performance tends to be pretty good which is not always the case for services like ChatGPT.

3. Customizability

When using a sesrvice like ChatGPT, CoPilot, Bard, you **might** have a few options of what model to run. [Ollama](https://ollama.com/library), LM Studio, and Jan.AI have a whole library of models to choose from. has a whole [library of models](https://ollama.com/library) to choose from, which can be used for different purposes. Some are general purpose models, some are specific to writing code, some are for creative purposes, some are for text generation, and more.

 4. Free

Ollama is free and open source. Paid services like ChatGPT, CoPilot, or Bard usually have a free tier of service but there are limitations to that. No such limits exist if you run it yourself. 

 5. Environmental Concerns

As the [Washington Post](https://www.washingtonpost.com/business/2024/06/21/artificial-intelligence-nuclear-fusion-climate/) explains, a massive amount of energy associated with Generative AI is being used today. AI servers are typically housed in large data centers which consume vast amounts of electricity. Training large AI models demands substantial computational power, running GPUs or TPUs (using parallell processing) for days or weeks. The electricity used by data centers often comes from non-renewable energy sources such as coal. Manufacturing the hardware used in electronics requires rare earth metals. And so on...

## Ollama

Ollama is an open source project that serves as a powerful and user-friendly platform for running LLMs on your local computer. Ollama simplifies the process of downloading, installing, and interacting with a wide range of LLMs.

### LM Studio

Download and use a "ChatGPT-Like" interface for running your model locally.

### Jan.AI


### Specific LLMs

Here are a few common ones that you might encounter. 

#### A note about "open" or "open source" models.

* [llama3](https://llama.meta.com/llama3/) - from Meta. Optimized for dialogue/chat use cases and 

* [qwen2](https://www.alibabacloud.com/blog/alibaba-cloud%E2%80%99s-qwen2-with-enhanced-capabilities-tops-llm-leaderboard_601268) - from AliBaba. Trained in many languages, not predominantly English. 

* [phi3](https://news.microsoft.com/source/features/ai/the-phi-3-small-language-models-with-big-potential/) - from Microsoft. A collection of models. 

* [mistral](https://mistral.ai/) - from Mistral AI. Optimized for business purposes

* [gemma](https://ai.google.dev/gemma) - from Google. A family of lightweight models


### HuggingFace

Train your own model!



