```
-Last updated 09/24/24
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
| Intro to Python pt 1                                                |       Wednesday 9/4   |  10:00 - 11:30am
| Intro to Python pt 2                                                |       Wednesday 9/11  |  10:00 - 11:30am
| Intro to Version Control w/ Git + Github                            |       Wednesday 9/11  |  1:00 - 2:30pm
| Python Data Analysis + Visualization                                |       Wednesday 9/18  |  10:00 - 11:30am
| Local Large Language Models                                         |       Wednesday 9/25  |  10:00 - 11:30am
| Python Web Scraping                                                 |       Wednesday 10/2  |  10:00 - 11:30am


# Disclaimer
I am not an AI expert! We are all learning and navigating this confusing landscape together. 


# Background Information 
## Large Language Models
A Large Language Model (LLM) is an artificial intelligence algorithm that uses deep learning techniques and massive data sets to understand and create human-like content across various media types including text, images, video, etc. These models are trained on extensive datasets of diverse information. Using deep learning techniques, they recognize patterns and relationships within and between different forms of media.

In simpler terms, an LLM is a computer program that has been fed enough examples of human language that it can recognize and interpret human language and other forms of complex data. Many LLMs are trained on data that has been gathered from the internet and the quality of the samples impacts how well the LLM will learn natural language. 

There are many LLMs in existence such as OpenAI's high profile GPT (Generative Pre-Trained Transformer). Some are optimized for specific purposes, as we will learn more about today, while others are more general use. 

LLMs are composed of large files that contain the parameters and architecture defining the model. These can be several gigabytes in size. Once the model is downloaded, it may need to be configured for a specific task. 


## Why?

With services available like ChatGPT and Copilot, you might be wondering why would you want to run an LLM directly on your own machine?

1. Customizability

When using a service like ChatGPT, Copilot, Bard, you **might** have a few options of what model to run. [Ollama](https://ollama.com/library), LM Studio, etc have a whole library of models to choose from, which can be used for different purposes. Some are general purpose models, some are specific to writing code, some are for creative purposes, some are for text generation, and more.

2. Privacy and Security

By processing information locally, your information remains secure and private. According to their [terms of service](https://openai.com/policies/terms-of-use/), OpenAI claims they are not keeping and misusing your data. However, there are concerns about that. UVA licenses [UVA Copilot](https://virginia.service-now.com/its?id=itsweb_kb_article&sys_id=8a0050d847fac610bb2b9c7b116d4317), an instance of Microsoft Copilot, which is probably safer to use. These concerns are negated if you run the LLM yourself!

3. Offline Use

At least with Ollama, if you have a scenario where the internet is not available, such as use in the field, you can still run your AI models because it is saved on your local machine. Similarly, performance tends to be pretty good which is not always the case for services like ChatGPT.

4. Free

The tools we will cover today are free and open source. Paid services like ChatGPT, Copilot, or Bard usually have a free tier of service but there are limitations to that. No such limits exist if you run it yourself. 

5. Environmental Concerns

As the [Washington Post](https://www.washingtonpost.com/business/2024/06/21/artificial-intelligence-nuclear-fusion-climate/) explains, a massive amount of energy associated with Generative AI is being used today. AI servers are typically housed in large data centers which consume vast amounts of electricity. Training large AI models demands substantial computational power, running for days or weeks. The electricity used by data centers often comes from non-renewable energy sources such as coal. Manufacturing the hardware used in electronics requires rare earth metals. And so on...

6. Local Development

This is more for developers, but downloading and running your own LLMs locally allow you a way to run them on a local server and integrate into an application you are writing. 

### [Ollama](https://ollama.com/)

Ollama is an open source project that serves as a powerful and user-friendly platform for running LLMs on your local computer. Ollama simplifies the process of downloading, installing, and interacting with a wide range of LLMs. See available models [here](https://github.com/ollama/ollama?tab=readme-ov-file#model-library).

### [LM Studio](https://lmstudio.ai/)

Download and use a "ChatGPT-Like" GUI interface to run your models locally. LM Studio makes it easy to download models, test them against each other, provides developer tools like running models on a local web server, etc. 


### Specific LLMs

Here are a few common ones that you might encounter. 

* [llama3](https://llama.meta.com/llama3/) - from Meta. Optimized for dialogue/chat use cases and 

* [qwen2](https://www.alibabacloud.com/blog/alibaba-cloud%E2%80%99s-qwen2-with-enhanced-capabilities-tops-llm-leaderboard_601268) - from AliBaba. Trained in many languages, not predominantly English. 

* [phi3](https://news.microsoft.com/source/features/ai/the-phi-3-small-language-models-with-big-potential/) - from Microsoft. A collection of models. 

* [mistral](https://mistral.ai/) - from Mistral AI. Optimized for business purposes

* [gemma](https://ai.google.dev/gemma) - from Google. A family of lightweight models


### Parameters

You will encounter this term when looking at the available LLMs and wonder what they are. To start with an example, think of the parameters like settings on a camera. You can adjust the camera's exposure, brightness, contrast, etc to get the perfect photo. Similarly, in machine learning, the parameters are adjusted within the model to optimize its performance for a specific task and direct the output/response accordingly. These adjustments help the model learn from data and make better predictions or decisions. The goal is the minimize the difference between the model's output and the actual correct outcome.  

When referring to a LLM, we also typically refer to the number of parameters that model contains. For example, ChatGPT contains around 175 billion parameters. This would be a massive file to download and install locally. Local LLMs are typically slimmed down versions of LLMs. There can be several versions of an LLM with different numbers of training parameters. 

### HuggingFace

[Hugging Face](https://huggingface.co/) is an open source data science and machine learning platform. It acts like Github but for AI. It is a place you can host and train your own AI models and datasets. A popular practice today is to take models that were trained on thousands of GPU hours and terabytes of data (such as LLama from Meta) and improve it further by adding new and refined data.

#### Use model from Hugging Face in Ollama

Yes, you can do it. [Here is a link to learn yourself](https://www.youtube.com/watch?v=fnvZJU5Fj3Q).



