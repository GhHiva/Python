spaCy has several pretrained language models which differ by:

- Language (e.g., English, German, etc.)

- Size (small = faster, large = more accurate)

- Components (e.g., POS tagging, NER, parsing, vectors)


| Model             | Size        | Features                                           | Speed       | Accuracy                |
| ----------------- | ----------- | -------------------------------------------------- | ----------- | ----------------------- |
| `en_core_web_sm`  | Small       | ✔ Tokenizer, POS, NER, Parsing (no word vectors)   | ⚡ Fast      | 👍 Good for quick tasks |
| `en_core_web_md`  | Medium      | ✔ Everything above + medium-sized **word vectors** | ⚖️ Balanced | Better                  |
| `en_core_web_lg`  | Large       | ✔ All components + **large word vectors**          | 🐢 Slower   | ✅ High                  |
| `en_core_web_trf` | Transformer | Uses **BERT-like transformer** (e.g., RoBERTa)     | 🧠 Slowest  | 💎 Highest accuracy     |

**How to See All Available Models: python -m spacy validate**
