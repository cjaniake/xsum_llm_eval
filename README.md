# XSum LLM Evaluation

[**XSum**](#xsum) | [**DeepEval**](#deepeval) | [**Colab Notebook**](./docs/getting_started.ipynb)

LLM evaluation is crucial for ensuring the stability and quality of your LLM application, whether it's a RAG system, an agent, a chatbot, or any other AI-driven solution. Robust evaluation frameworks help assure that the system behaves as expected in a variety of scenarios and that improvements in one use case don’t inadvertently break another.  

It enables a shift from subjective to objective evaluation, providing measurable benchmarks to assess changes in different components, such as the underlying LLM model, prompts, retrieval mechanisms, and more. By systematically assessing aspects like factual accuracy, coherence, and robustness to adversarial inputs, you can fine-tune your models, improve user experience, and maintain trust in your application’s reliability.  

In this project, we will use the XSum summarization dataset as an example to demonstrate LLM evaluation in practice. XSum provides a challenging benchmark for evaluating the quality of generated summaries, making it a suitable choice for testing different evaluation approaches. By leveraging DeepEval, we aim to illustrate how systematic evaluation can help ensure model reliability and guide improvements in different components of an LLM application.

# <a name="xsum"></a>XSum

The XSum (Extreme Summarization) dataset is a large-scale corpus designed for abstractive text summarization, focusing on generating highly concise, one-sentence summaries that answer the question, "What is the article about?".  

Unlike traditional summarization datasets that often align with extractive strategies, XSum emphasizes abstraction, requiring models to generate novel phrasings rather than copying directly from the source text. The dataset was constructed by harvesting news articles from the British Broadcasting Corporation (BBC), where the first sentence of each article’s professionally written summary serves as the reference summary.  

This setup presents a challenging benchmark for evaluating the ability of models to perform extreme summarization with minimal redundancy while preserving the core meaning of the article.

Explore the dataset using [HuggingFace Datasets](https://huggingface.co/datasets/EdinburghNLP/xsum) Dataset Viewer.

# <a name="deepeval"></a>DeepEval

DeepEval is an open-source evaluation framework designed to streamline the assessment and iteration of LLM applications. It simplifies the process of "unit testing" LLM outputs, much like Pytest does for traditional code, allowing developers to validate and refine their solution efficiently. DeepEval comes with over 14 built-in evaluation metrics, enabling users to measure various aspects of LLM performance with minimal effort.  

Additionally, DeepEval supports Red Teaming, enabling developers to identify safety risks and vulnerabilities in LLM applications by evaluating their responses to adversarial attacks. It also includes synthetic dataset generation powered by state-of-the-art evolution techniques, helping developers build test cases from their knowledge base input data.  


