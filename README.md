# 🧠 LLM Mechanisms — Personal Learning Path

A personal notebook + script collection for understanding how Large Language Models work from the inside out. Built as I learn — expect rough edges, experiments, and a lot of comments.

---

## 📁 Structure

```
lllm-mechanisms-learning-path/
│
├── Part1_TokensEmbeddings/
│   ├── text2numbers/
│   │   ├── part1_text2num_preparingText.ipynb
│   │   ├── part1_text2num_buildingVocab.ipynb
│   │   └── vocab_builder.py
│   ├── embeddings/
│   │   ├── part1_embeddings_word2vec.ipynb
│   │   ├── part1_embeddings_positional.ipynb
│   │   └── part1_embeddings_viz.ipynb
│   └── sentence_embeddings/
│       ├── part1_sentenceEmbeddings_cosineSim.ipynb
│       └── part1_sentenceEmbeddings_multilingual.ipynb
│
├── Part2_AttentionTransformers/
│   ├── part2_attention_scaledDotProduct.ipynb
│   ├── part2_attention_multiHead.ipynb
│   ├── part2_transformer_encoderBlock.ipynb
│   ├── part2_transformer_decoderBlock.ipynb
│   └── part2_transformer_fullModel.ipynb
│
├── Part3_TrainingFineTuning/
│   ├── part3_training_pretrainingObjectives.ipynb
│   ├── part3_training_fromScratch.ipynb
│   ├── part3_finetuning_supervised.ipynb
│   ├── part3_finetuning_lora.ipynb
│   └── part3_training_rlhf_notes.ipynb
│
├── Part4_RAGApplications/
│   ├── part4_rag_basicPipeline.ipynb
│   ├── part4_rag_faissIndexing.ipynb
│   ├── part4_rag_langchain.ipynb
│   └── faiss_store.py
│
├── Part5_MechanisticInterpretability/
│   ├── part5_interp_attentionPatterns.ipynb
│   ├── part5_interp_logitLens.ipynb
│   ├── part5_interp_activationPatching.ipynb
│   └── part5_interp_probing.ipynb
│
└── utils/
    ├── tokenizer_utils.py
    └── viz_utils.py
```

---

## 🗺️ Learning Path

| # | Topic | Key Concepts |
|---|-------|-------------|
| 1 | **Tokenization & Vocab** | BPE, WordPiece, word2idx, special tokens |
| 2 | **Embeddings** | Dense vectors, Word2Vec, positional encoding, sentence embeddings |
| 3 | **Attention & Transformers** | Self-attention, multi-head, encoder-decoder, BERT vs GPT |
| 4 | **Training & Fine-tuning** | MLM, CLM, supervised fine-tuning, RLHF |
| 5 | **RAG & Applications** | Vector stores, retrieval, FAISS, LangChain |
| 6 | **Mechanistic Interpretability** | Attention viz, logit lens, activation patching |

---

## 🛠️ Stack

- **Language** — Python 3.10+
- **Deep Learning** — PyTorch
- **NLP** — HuggingFace Transformers, sentence-transformers
- **Vector Search** — FAISS
- **Orchestration** — LangChain
- **Viz** — matplotlib, UMAP, BertViz
- **Package Manager** — uv

---

## ⚙️ Setup

```bash
git clone https://github.com/ishan-chowdhury/llm-mechanisms-learning-path
cd llm-mechanisms-learning-path

uv venv
source .venv/bin/activate
uv pip install -r requirements.txt
```

---

## 📌 Notes

- Notebooks are messy by design — they're for understanding, not production
- Each section has a `_scratch` notebook where I experiment before cleaning up
- Comments are verbose on purpose

---

## 📚 References & Inspiration

- [Mike X Cohen — LLM Course](https://github.com/mikexcohen/LLM_course)
- [Andrej Karpathy — nanoGPT](https://github.com/karpathy/nanoGPT)
- [Jay Alammar — Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)
- [Neel Nanda — Mechanistic Interpretability](https://www.neelnanda.io/mechanistic-interpretability)
- [mlabonne — LLM Course](https://github.com/mlabonne/llm-course)

---

*Personal notes repo — not a tutorial, not production code. Just learning in public.*
