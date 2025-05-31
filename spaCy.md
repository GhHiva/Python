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

**How to See All Available Models:** `python -m spacy validate`

**How to download a model:** `python -m spacy download en_core_web_md`

**Use in Python:**     

import spacy

`nlp = spacy.load("en_core_web_md")`


### spaCy attributes:
- `.is_stop`: Returns True if the token is a stop word (like "a", "and", "the", "in", etc.)
- `.is_punct`: Returns True if the token is punctuation (e.g., ., ,, !, :)
- `.lemma_`: Gives the base form (lemma) of the word. (Example: “running” → “run”, “mice” → “mouse”)
