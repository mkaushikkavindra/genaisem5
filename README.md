# GenAI & LLM Laboratory

## Overview

This repository contains the implementation and execution results of
**12 Generative AI and Large Language Model (LLM) laboratory
experiments**. The experiments cover foundation models, prompt
engineering, conversational AI, text generation, retrieval-augmented
generation, code generation, image generation, multimodal AI,
fine-tuning, multimedia content generation, and deployment/evaluation.

The experiments were executed primarily using **Google Colab**, with GPU
acceleration used where required for computationally intensive models.

## Objectives

The laboratory experiments are designed to provide practical exposure
to:

-   Pre-trained foundation models and LLMs
-   Prompt engineering techniques
-   Conversational AI and chatbots
-   Text summarization and question answering
-   Sentiment analysis and document classification
-   Retrieval-Augmented Generation (RAG)
-   AI-assisted code generation and debugging
-   Diffusion-based image generation
-   Multimodal AI
-   Fine-tuning pre-trained language models
-   AI-based text, image, and audio generation
-   Deployment and evaluation of Generative AI applications

## Experiments

### Experiment 1 --- Text Generation Using Pre-Trained Foundation Models

A pre-trained **GPT-2** model is used to generate text from a given
prompt. The experiment demonstrates text generation and sampling-based
decoding techniques.

**Key concepts:** - Pre-trained foundation models - Text generation -
Temperature - Top-k sampling - Top-p (nucleus) sampling

**Model:** GPT-2

------------------------------------------------------------------------

### Experiment 2 --- Prompt Engineering Techniques

Different prompting strategies are explored to understand how prompt
design affects the behavior of a language model.

**Techniques covered:** - Zero-shot prompting - Few-shot prompting -
Chain-of-Thought (CoT) prompting

The outputs of different prompting approaches are compared to understand
their effect on model responses.

------------------------------------------------------------------------

### Experiment 3 --- Conversational AI Chatbot

A multi-turn conversational chatbot is implemented using **DialoGPT**.
The chatbot maintains conversation history so that responses can be
generated based on previous turns.

**Key concepts:** - Conversational AI - Transformer-based dialogue
models - Multi-turn conversation - Conversation context

**Model:** Microsoft DialoGPT-medium

------------------------------------------------------------------------

### Experiment 4 --- Text Summarization and Question Answering

Two natural language processing applications are implemented:

1.  **Text summarization** using BART
2.  **Extractive question answering** using DistilBERT trained on SQuAD

The experiment demonstrates how pre-trained transformer models can
perform different language understanding tasks.

**Models:** - `facebook/bart-large-cnn` -
`distilbert-base-cased-distilled-squad`

------------------------------------------------------------------------

### Experiment 5 --- Sentiment Analysis and Document Classification

Pre-trained transformer models are used for:

-   Sentiment analysis of text reviews
-   Zero-shot document classification

The experiment demonstrates how language models can classify text
without training a new model specifically for the classification task.

**Models:** - DistilBERT sentiment model - BART-large-MNLI

------------------------------------------------------------------------

### Experiment 6 --- Retrieval-Augmented Generation (RAG) Using FAISS

A basic RAG system is implemented by combining:

-   Document embeddings
-   FAISS vector similarity search
-   Retrieved contextual information
-   A text generation model

The system retrieves relevant information from a small knowledge base
and uses that information to generate a grounded response.

**Key concepts:** - Embeddings - Vector search - FAISS - Retrieval -
Context augmentation - Grounded generation

**Models/Tools:** - Sentence Transformers (`all-MiniLM-L6-v2`) - FAISS -
FLAN-T5

------------------------------------------------------------------------

### Experiment 7 --- AI-Powered Code Generation and Debugging Assistant

A pre-trained code language model is used to generate programming code
from natural-language instructions and assist with debugging a faulty
program.

**Tasks demonstrated:** - Natural-language-to-code generation - Code
completion - Code debugging

**Model:** Salesforce CodeGen-350M-mono

------------------------------------------------------------------------

### Experiment 8 --- Image Generation Using Diffusion Models

A text-to-image generation system is implemented using a **Stable
Diffusion** model.

A natural-language prompt is provided to the model, which generates a
corresponding image.

**Key concepts:** - Diffusion models - Text-to-image generation -
Prompt-based image generation - Inference steps - Guidance scale

**Model:** Stable Diffusion v1.5

**Hardware:** GPU recommended

------------------------------------------------------------------------

### Experiment 9 --- Multimodal AI Application

A multimodal AI application is developed using **BLIP** to process image
and text information.

The experiment demonstrates:

-   Image caption generation
-   Visual Question Answering (VQA)

The model receives an image and can generate a textual description or
answer a question about the image.

**Model:** Salesforce BLIP

------------------------------------------------------------------------

### Experiment 10 --- Fine-Tuning a Pre-Trained Language Model

A pre-trained **DistilBERT** model is fine-tuned for sentiment
classification using the **IMDB dataset**.

The experiment demonstrates the transfer-learning workflow:

1.  Load a pre-trained model
2.  Prepare a labeled dataset
3.  Tokenize the data
4.  Fine-tune the model
5.  Evaluate performance
6.  Save the fine-tuned model

**Dataset:** IMDB

**Model:** DistilBERT

**Hardware:** GPU recommended

------------------------------------------------------------------------

### Experiment 11 --- AI-Based Multimedia Content Generation

An integrated Generative AI workflow is developed to generate multiple
types of content from a single topic:

-   Text
-   Image
-   Audio

The experiment combines language generation, image generation, and
text-to-speech technologies.

**Models/Tools:** - FLAN-T5 for text generation - Stable Diffusion for
image generation - gTTS for audio generation

This demonstrates how different generative models can be combined into a
single content-generation pipeline.

------------------------------------------------------------------------

### Experiment 12 --- Deployment and Evaluation of a Generative AI Application

A text summarization application is developed and deployed as an
interactive web interface using **Gradio**.

The generated summaries are also evaluated using **ROUGE metrics**.

**Key concepts:** - Generative AI application deployment - Interactive
web interfaces - Text summarization - Automatic evaluation - ROUGE

**Tools/Models:** - BART - Gradio - ROUGE

------------------------------------------------------------------------

## Technologies Used

The experiments use a combination of the following technologies and
libraries:

-   Python
-   Google Colab
-   PyTorch
-   Hugging Face Transformers
-   Hugging Face Diffusers
-   Datasets
-   Sentence Transformers
-   FAISS
-   Gradio
-   Evaluate / ROUGE
-   gTTS
-   Pillow

## Execution Environment

**Google Colab** is used as the primary execution environment because it
provides a convenient Python environment and access to GPU acceleration.

GPU acceleration is particularly useful for computationally intensive
experiments such as:

-   Stable Diffusion image generation
-   DistilBERT fine-tuning
-   Multimedia generation involving diffusion models

Experiments that do not require significant GPU computation can also be
executed using a CPU runtime.

## Outputs

The notebooks contain the executed programs along with their generated
outputs. Depending on the experiment, outputs include:

-   Generated text
-   Chatbot responses
-   Summaries
-   Question-answering results
-   Classification results
-   Retrieved RAG context
-   Generated code
-   Generated images
-   Image captions
-   VQA answers
-   Training and evaluation metrics
-   Generated audio
-   Gradio application output
-   ROUGE evaluation scores

## Important Note on Model Outputs

Generative AI models are probabilistic systems. Therefore, generated
text, images, chatbot responses, and code may vary between executions
depending on model versions, sampling settings, random seeds, and
runtime environments.

The implementations in this repository follow the laboratory experiments
and use compatibility adjustments only where necessary to execute the
experiments with current software environments.

## Learning Outcomes

After completing these experiments, the following practical concepts are
demonstrated:

-   Working with pre-trained foundation models
-   Designing effective prompts
-   Building conversational AI systems
-   Performing common NLP tasks
-   Implementing a basic RAG pipeline
-   Using vector embeddings and similarity search
-   Applying LLMs to programming tasks
-   Generating images from text prompts
-   Building multimodal AI applications
-   Fine-tuning transformer models
-   Combining multiple generative AI models
-   Deploying Generative AI applications
-   Evaluating generated text using automatic metrics

## Conclusion

This laboratory provides a practical introduction to modern Generative
AI and LLM technologies. The experiments progress from basic text
generation and prompting to more advanced applications such as RAG,
multimodal AI, model fine-tuning, multimedia generation, and deployment.

The repository serves as a record of the implementation, execution, and
outputs of all 12 laboratory experiments.
