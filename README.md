# SEARAG: Semantic Entropy-Guided Adaptive Retrieval for Multi-hop Question Answering 🔍🔄

**English** | [中文](README_zh.md)

> **Note: Code Release Schedule** 📅🔒➡️🔓
>
> This repository contains the code for our paper submitted to **ICASSP 2026**.
>
> In accordance with the **single-blind review policy**, the full code implementation will be made publicly available **immediately upon acceptance** of the paper.
>
> **We are committed to open science and will release our code without fail!** ✅

---

## 📝 Paper Information

**Title:** SEARAG: Semantic Entropy-Guided Adaptive Retrieval for Multi-hop Question Answering

**Authors:** Dingfu Yu, Qinhong Lin, Zhongliang Yang*, Linna Zhou  
**Affiliation:** School of Cyberspace Security, Beijing University of Posts and Telecommunications  
**Conference:** ICASSP 2026 (Under Review)

**Abstract:** Retrieval-Augmented Generation (RAG) enhances Large Language Models (LLMs) in knowledge-intensive tasks, but static retrieval strategies fail to adapt to evolving informational needs. We propose SEARAG, which trains a discriminative model to predict binary semantic entropy from hidden-layer states, quantifying uncertainty in real time. During generation, we use iterative sentence-by-sentence reasoning to dynamically trigger retrieval when high semantic entropy is detected.

## 🚀 Coming Soon

Upon acceptance, this repository will contain:

- ✅ **Complete training code** for semantic entropy prober
- ✅ **Inference implementation** of SEARAG framework
- ✅ **Step-by-step guide** for prober training and evaluation
- ✅ **Experiment scripts** for reproducing all results in the paper
- ✅ **Uncertainty-aware query formulation** and reranking implementation

## 🏗️ Method Overview

SEARAG introduces three key innovations:

1. **🧠 Semantic Entropy Prober**: Lightweight MLP classifier trained to predict uncertainty from LLM hidden states
2. **💡 Uncertainty-aware Query Formulation**: Dynamically identifies uncertain words and formulates targeted retrieval queries
3. **🎯 Adaptive Reranking**: Refines retrieval results based on real-time uncertainty signals

## 📊 Experimental Results

SEARAG outperforms existing adaptive RAG methods across **five multi-hop QA datasets**:

- **In-domain**: 2WikiMultiHopQA, HotpotQA, IIRC
- **Out-of-domain**: MuSiQue, FRAMES
- **Models**: Llama2-13B, Llama3.1-8B, Mistral-7B

## 🛠️ Requirements

*(To be detailed upon release)*
- Python ≥ 3.8
- PyTorch
- Transformers
- Standard NLP libraries

## 📄 Citation

If you find our work useful, please cite our paper upon its acceptance:

```bibtex
@inproceedings{yu2026searag,
  title={SEARAG: Semantic Entropy-Guided Adaptive Retrieval for Multi-hop Question Answering},
  author={Yu, Dingfu and Lin, Qinhong and Yang, Zhongliang and Zhou, Linna},
  booktitle={ICASSP 2026 - IEEE International Conference on Acoustics, Speech and Signal Processing},
  year={2026}
}
