# Language-Modelling-on-Indian-names
The goal is to understand the evolution of statistical language models (N-grams) to neural language models (Feedforward &amp; RNNs), and evaluate their ability to model sequences.
🚀 Models Implemented

Unigram Language Model

Assumes characters are independent.

Baseline model; poor quality output.

Bigram Language Model

Conditions each character on the previous one.

Captures local dependencies like “th” or “sh”.

Trigram Language Model

Considers the previous two characters.

Better sequence coherence than bigram.

Neural N-gram Language Model

Feedforward NN with embeddings for previous n characters.

Learns smoother distributions, reduces sparsity.

RNN Language Model

Recurrent Neural Network processes sequences step-by-step.

Captures long-range dependencies, produces most realistic names.
