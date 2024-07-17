# llm_path.github.io


# DAY-1
Video Link : https://youtu.be/MyFrMFab6bo?list=PL1T8fO7ArWleyIqOy37OVXsP4hFXymdOZ 
- NN operations are just matrix multiplications.
- GPUs are really fast at matrix multiplications.
- Validation set is for
  -   ensuring that training is not "overfitting"
  -   setting hyper-parameters of the
model (e.g. number of parameters)
- Before ~2020: each task had its own NN architecture ; Now Transformers.
- ## Transformer Summary
  - Inputs
     - Inputs need to be vectors of numbers
     - Start with original text:
     - "It's a blue sundress."
     - Turn into a sequence of tokens:
     - [<SOS>, It, 's, a, blue, sund, ress, ., <EOS>]
     - Turn into vocabulary IDs:
     - [0, 1026, 338, 257, 4171, 37437, 601, 13, 1]
     - Each ID can be represented by a one-hot vector
     - e.g. 3 -> [0, 0, 0, 1, 0, 0, 0, 0, ...]
   - Input Embedding
     - One-hot vectors are poor representations of words or tokens 
     – e.g. distance between "cat" and "kitten" is the same as between "cat" and "tractor"
     - Solution: learn an embedding matrix!
   - Attention
     - Key insight: for a given token in the output sequence, only one or a few tokens in the input sequence are most important.
  - Basic self-attention
    - Input: sequence of vectors X1, X2,... Xt
    - Output: sequence of vectors, each one a weighted sum of the input sequence Y1 Y2,... Yt Y₁ = Σ WijxXj q ,k , v 
  - Masked Multi head attention
    - Conceptual view:
      - token comes in
      - gets "augmented" with previously-seen tokens that seem relevant (masked self-attention)
      - this happens in several different ways simultaneously (multiple heads)
   - Then positional encoding, add,
   - Normalization:
 
 - ## Introduction to LLM: 
     -  BERT, T5, GPT2
     -  GPT3 : Just like GPT-2 but 100x larger. Zero shot, one-shot, few-shot.
     -  LLaMA : Training dataset: Wikipedia, Github, Books, ArXiv etc.
     -  https://fullstackdeeplearning.com/
- ## Reading Series
     -  https://github.com/aishwaryanr/awesome-generative-ai-guide/blob/main/free_courses/Applied_LLMs_Mastery_2024/week1_part1_foundations.md
     -  let's break down what "Language Models" mean in this context. Language models are essentially algorithms or systems that are trained to understand and generate human-like text. They serve as a representation of how language works, learning from diverse datasets to predict what words or sequences of words are likely to come next in a given context. The "Large" aspect amplifies their capabilities. Traditional language models, especially those from the past, were smaller in scale and couldn't capture the intricacies of language as effectively. With advancements in technology and the availability of massive computing power, we've been able to build much larger models. These Large Language Models, like ChatGPT, have billions of parameters, which are essentially the variables the model uses to make sense of language.
 
     -  
