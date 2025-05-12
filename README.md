# NLP

**Regular Expression: (Regex)**

Regular expressions are strings you can use that have a special syntax, which allows you to match patterns and find other strings. 
A pattern is a series of letters or symbols which can map to an actual text or words or punctuation. You can use regular expressions to do things like find links in a webpage, parse email addresses and remove unwanted strings or characters. 
The syntax for the regex library is always to pass the pattern first, and the string second.





# Transformers

Transformer architecture consists of two blocks:

**Encoder:**
   The encoder block consists of multiple identical layers that are responsible for reading and processing the entire input sequence, generating context-rich numerical representations.
   It does this using self-attention and feed-forward networks.

**Decoder:**
   The decoder block essentially does the inverse of the encoder block, generating an output sequence based on the encoded input sequence.
   
**Positional Encodings:**
     Key to both encoder and decoder blocks is positional, which allows tokens to be processed in parallel by encoding each token's position in the sequence. 
     This enables the model to recognize the relationships between tokens and their order, essential for making sense of sentences and capturing their context.

**Attention Mechanism:**

 Attention mechanisms are used to focus on the most important tokens and their relationships, which improves the quality of generated text.

 Self-attention is a type of attention mechanism that assigns a weight to each token in the sequence simultaneously, capturing long-range dependencies.

 Multi-head attention extends self-attention by using multiple "heads" to focus on different aspects of the input sequence in parallel. This allows each head to capture distinct relational 
 patterns within the data, leading to richer representations that enhance LLMs' effectiveness across tasks.

 **Position-Wise feed forward Neural networks:**
 
 These are simple neural networks that apply complex transformations on each token's embeddings independently. 
 Because each token gets its own transformation, the networks are position- independent, hence, the "position-wise".

