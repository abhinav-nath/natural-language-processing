# BERT

BERT began rolling out in Google's search system the week of October 21, 2019 for English-language queries.

BERT stands for **B**idirectional **E**ncoder **R**epresentations from **T**ransformers, is a neural network-based technique for NLP **pre-training**.
In plain English, it can be used to help Google better discern the context of words in search queries.

For example, in the phrases *"nine to five"* and *"a quarter to five"*, the word *"to"* has two different meanings, which may be obvious to humans but less so to search engines. BERT is designed to distinguish between such nuances to facilitate more relevant results.

Google open-sourced BERT in November 2018.
This means that anyone can use BERT to train their own language processing system for question answering or other tasks.

## How does BERT work?

The breakthrough of BERT is in its ability to train language models based on the entire set of words in a sentence or query (bidirectional training) rather than the traditional way of training on the ordered sequence of words (left-to-right or combined left-to-right and right-to-left).
BERT allows the language model to learn word context based on surrounding words rather than just the word that immediately precedes or follows it.

For example, the word *"bank"* would have the same context-free representation in *"bank account"* and *"bank of the river"*. Contextual models instead generate a representation of each word that is based on the other words in the sentence. For example, in the sentence *"I accessed the bank account"*, a unidirectional contextual model would represent *"bank"* based on *"I accessed the"* but not *"account"*. However, BERT represents *"bank"* using both its previous and next context — *"I accessed the ... account"*.