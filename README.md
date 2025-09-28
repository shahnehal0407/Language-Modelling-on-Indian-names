#  Assignment 2: Language Modelling (DS207 – Intro to NLP)

##  Overview
This project implements and compares **character-level language models** to generate city names.  
The assignment was part of the **Intro to NLP (DS207)** course at IISc, guided by TA Yash Patel.  

The goal is to understand the evolution of **statistical language models (N-grams)** to **neural language models (Feedforward & RNNs)**, and evaluate their ability to model sequences.



# Models Implemented
1. **Unigram Language Model**  
   - Assumes characters are independent.  
   - Baseline model; poor quality output.  

2. **Bigram Language Model**  
   - Conditions each character on the previous one.  
   - Captures local dependencies like “th” or “sh”.  

3. **Trigram Language Model**  
   - Considers the previous two characters.  
   - Better sequence coherence than bigram.  

4. **Neural N-gram Language Model**  
   - Feedforward NN with embeddings for previous *n* characters.  
   - Learns smoother distributions, reduces sparsity.  

5. **RNN Language Model**  
   - Recurrent Neural Network processes sequences step-by-step.  
   - Captures long-range dependencies, produces most realistic names.  



# Evaluation
- **Metric:** Perplexity (lower = better).  
- **Qualitative:** Generate novel city names and compare realism.  

# Expected Results:
- **Unigram:** Random nonsense (no structure).  
- **Bigram/Trigram:** Some structure (e.g., "Delhi" → "Dehli").  
- **Neural N-gram:** More fluent, fewer nonsense names.  
- **RNN:** Best performance, produces realistic new names.  

# Setup & Running
Clone this repo and install dependencies:
```bash
git clone https://github.com/yourusername/language-modelling-assignment.git
cd language-modelling-assignment
pip install torch==2.3.0 torchtext==0.18 pandas numpy
```

Run the notebook in Jupyter/Colab:
```bash
jupyter notebook Assignment_2_Language_Modelling.ipynb
```


# Sample Outputs
*(replace with your actual generated outputs)*

- **Unigram:** `axxq, lrrpa, oottm`  
- **Bigram:** `Dehli, Kolcata, Bombey`  
- **Trigram:** `Bangaluru, Hydrabad`  
- **Neural N-gram:** `Ahmednagr, Suratpur`  
- **RNN:** `Chandrapura, Vishakhapatnam`  

#  Learnings
- Understood trade-offs between **statistical** vs **neural** models.  
- Observed **data sparsity problem** in N-grams and how neural embeddings help.  
- Practiced **PyTorch implementation** of feedforward and recurrent LMs.  
- Learned evaluation using **perplexity** and **sample-based qualitative analysis**.  

---

