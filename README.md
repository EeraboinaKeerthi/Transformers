# NLP

**Preprocessing steps:**

1. Tokenization
   
2. Stemming/Lemmatization : shorten words to their root stems.
   
3. Removal of stop words


**Regular Expression: (Regex)**

Regular expressions are strings you can use that have a special syntax, which allows you to match patterns and find other strings. 
A pattern is a series of letters or symbols which can map to an actual text or words or punctuation. You can use regular expressions to do things like find links in a webpage, parse email addresses and remove unwanted strings or characters. 
The syntax for the regex library is always to pass the pattern first, and the string second.

**Tokenization**
Tokenization is the process of transforming a string or document into smaller chunks, which we call tokens. 

Why bother with tokenization? 

Because it can help us with some simple text processing tasks like mapping part of speech, matching common words and perhaps removing unwanted tokens like common words or repeated words. 

sent_tokenize function will split a document into individual sentences. 

The regexp_tokenize uses regular expressions to tokenize the string, giving you more granular control over the process. 

And the tweettokenizer does neat things like recognize hashtags, mentions and when you have too many punctuation symbols following a sentence.

**Topic Identification**

Using basic NLP models, will identify topics from texts based on term frequencies. 

Two simple methods: bag-of-words and Tf-idf

**Bag-of-words:**

Bag of words is a very simple and basic method to finding topics in a text. 

For bag of words, you need to first create tokens using tokenization, and then count up all the tokens you have. 

The theory is that the more frequent a word or token is, the more central or important it might be to the text. 

Bag of words can be a great way to determine the significant words in a text based on the number of times they are used.

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

