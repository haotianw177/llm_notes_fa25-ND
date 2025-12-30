<!-- #! ariamis -->

# notes 

## short q&a

In language modeling, the pretraining phase is self-supervised, meaning that labels are obtained automatically from raw text, such as masking a word for prediction.

GPT-1 pre-trained on Next word prediction

BART, T5, GPT could be used for this task setup of: 1. Input: STEM lecture recording 2. Output: A multiple-choice quiz question

about transformers: 1. Without a positional encoding layer for transformer-based architectures, the architecture cannot make sense of the order of tokens 2. Transformers are the backbone behind models like BERT, GPT, and T5 3. Bidirectional transformer-based architectures like BERT are good at context understanding, while unidirectional transformer-based architectures like GPT can generate text well.

The scaling law in neural language models (LM) is mainly concerned with the effect of which of the following factors on the performance of LMs? 1. Number of parameters 2. Compute budget 3. Number of training tokens

The Chinchilla Scaling Law is concerned with scaling model size and data size proportionally to achieve compute-optimal performance

What is the major weakness of fine tuning language models for specific tasks? It requires a large label data set for each task and runs into generalization issues.

Which of the following statements is NOT a potential explanation for the effectiveness of in-context learning? The training examples provided in the prompt allow us to update the parameters of the LLMs to adapt to the downstream tasks

In recent LLMs, the term “expert” in Mixture-of-Experts refers to a small subset of parameters of the model that are activated during processing

The design of an MOE architecture depends on the following factors: The size of an expert, The number of experts, The frequency with which MoEs are inserted (every layer, every other layer, etc.) it's not depend: The diversity of the training data to ensure the non-overlapping knowledge of the experts

Which of the following is TRUE about Mixture of Experts (MOEs): The use of load balancing loss prevents unused “dead weights” that take up GPU memory.





## long questions

What are the scaling laws for language models? Estimate the data size and compute required to train GPT-3.

What are the key differences between In-Context Learning (ICL) and Supervised Learning?

What is the main idea behind a sparse Mixture of Experts (MoE) model? What makes it different from a dense model?

Provide an example of an LLM that makes use of Mixture of Experts (MoE). Using the LLM as a case study, explain how MoE helps improve performance and efficiency.

How does Chain-of-Thought (CoT) help improve the performance of LLM on reasoning tasks?

What are the advantages and disadvantages of using more complex thought structures, like Tree-of-Thought (ToT) or Graph-of-Thought (GoT), in LLMs?

