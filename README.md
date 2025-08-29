# 🇬🇧→🇯🇵 English to Japanese Transformer

This project is a **from-scratch Transformer neural network** (built with PyTorch) that translates English sentences into Japanese.  
I built it as a project to gain a deep understanding of how Transformers are constructed and trained. By implementing everything from scratch (without Hugging Face), I was able to break down and visualize each component of the architecture, understand why it’s important, and explore different ways to optimize the model for speed and efficiency.

---

## How the Project Works

- Loads and cleans an English–Japanese dataset (from [Tatoeba](https://tatoeba.org/en/sentences/search?from=jpn&to=eng))
- Trains a **SentencePiece tokenizer** for subword encoding
- Implements a custom **Transformer encoder–decoder** with `nn.Transformer`
- Trains with **teacher forcing**, **label smoothing**, and **BLEU evaluation**
- Includes demo code to translate sentences from English → Japanese

---

## Quickstart

1. **Clone this repo:**

   ```bash
   git clone https://github.com/devinjudson/enja-transformer.git
   cd enja-transformer
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook:**

   ```bash
   jupyter notebook enja_transformer.ipynb
   ```

---

## Example

After training, you can run:

```python
greedy_decode("hello, how are you?")
# => こんにちは、お元気ですか？
```

---

## What I Learned

- How to preprocess bilingual data and train a subword tokenizer
- How the Transformer architecture (attention, encoder–decoder) works in practice
- Training workflows in PyTorch (teacher forcing, validation, BLEU evaluation)
- How to save and resume training with checkpoints
- Techniques for efficient training and optimization
- Why dataset size has such a strong impact on translation quality

---
