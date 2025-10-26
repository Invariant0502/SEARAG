# SEARAG: 基于语义熵的自适应检索多跳问答 🔍🔄

[English](README.md) | **中文**

> **注意：代码发布计划** 📅🔒➡️🔓
>
> **本代码库包含我们提交至ICASSP 2026的论文相关代码。**
>
> 完整代码将在**论文接收后立即公开**。
>
> **我们致力于开放科学，一定会公开代码！** ✅

---

## 📝 论文信息

**标题：** SEARAG: Semantic Entropy-Guided Adaptive Retrieval for Multi-hop Question Answering

**作者：** 俞定甫, 林钦鸿, 杨忠良*, 周琳娜  
**单位：** 北京邮电大学网络空间安全学院  
**会议：** ICASSP 2026 (评审中)

**摘要：** 检索增强生成(RAG)增强了大型语言模型在知识密集型任务中的表现，但静态检索策略无法适应不断变化的信息需求。我们提出了SEARAG，它训练一个判别模型从隐藏层状态预测二元语义熵，实时量化不确定性。在生成过程中，我们使用逐句迭代推理，在检测到高语义熵时动态触发检索。

## 🚀 即将公开

论文接收后，本仓库将包含：

- ✅ **完整的语义熵探测器训练代码**
- ✅ SEARAG框架的**推理实现**
- ✅ **多跳问答数据集**预处理脚本
- ✅ 探测器训练和评估的**详细指南**
- ✅ 复现论文所有结果的**实验脚本**
- ✅ **不确定性感知查询构建**和重排序实现

## 🏗️ 方法概述

SEARAG引入三个关键创新：

1. **🧠 语义熵探测器**：轻量级MLP分类器，训练用于从LLM隐藏状态预测不确定性
2. **💡 不确定性感知查询构建**：动态识别不确定词并构建针对性检索查询
3. **🎯 自适应重排序**：基于实时不确定性信号优化检索结果

## 📊 实验结果

SEARAG在**五个多跳问答数据集**上优于现有自适应RAG方法：

- **域内数据集**：2WikiMultiHopQA, HotpotQA, IIRC
- **域外数据集**：MuSiQue, FRAMES
- **模型**：Llama2-13B, Llama3.1-8B, Mistral-7B

## 🛠️ 环境要求

*(接收后详细说明)*
- Python ≥ 3.10
- PyTorch
- Transformers
- 标准NLP库

## 📄 引用

如果我们的工作对您有帮助，请在论文接收后引用：

```bibtex
@inproceedings{yu2026searag,
  title={SEARAG: Semantic Entropy-Guided Adaptive Retrieval for Multi-hop Question Answering},
  author={Yu, Dingfu and Lin, Qinhong and Yang, Zhongliang and Zhou, Linna},
  booktitle={ICASSP 2026 - IEEE International Conference on Acoustics, Speech and Signal Processing},
  year={2026}
}
