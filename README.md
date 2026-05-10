# BERT-GPT2 Contrast

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Deep Learning](https://img.shields.io/badge/Deep%20Learning-PyTorch-red.svg)](https://pytorch.org/)
[![NLP](https://img.shields.io/badge/NLP-Hugging%20Face-green.svg)](https://huggingface.co/)

## English

A practical comparison project between **BERT** (bidirectional encoder) and **GPT-2** (unidirectional decoder) transformer architectures. This project demonstrates the fundamental differences in pre-training objectives and downstream task performance.

### Quick Start

```bash
# 1. Install dependencies
pip install torch transformers datasets

# 2. Login to Hugging Face and download models
# Visit https://huggingface.co/ to register

# 3. Run notebooks
jupyter notebook bert_gpt2.ipynb          # Basic comparison
jupyter notebook bert_gpt2_GLUE.ipynb    # GLUE benchmark evaluation
```

## 中文

**BERT-GPT2 对比项目** — 一个专注于 BERT 与 GPT-2  transformer 架构对比的实践项目。项目包含基础对比代码和 GLUE 基准评测两套notebook，直观展示两种架构在预训练目标和下游任务中的差异。

### 快速开始

```bash
# 第1步：安装依赖
pip install torch transformers datasets

# 第2步：登录 Hugging Face 下载模型和数据
# 访问 https://huggingface.co/ 注册账号

# 第3步：运行notebook
jupyter notebook bert_gpt2.ipynb          # 基础对比
jupyter notebook bert_gpt2_GLUE.ipynb    # GLUE基准评测
```

## Core Features | 核心特性

| Feature | BERT | GPT-2 |
|---------|------|-------|
| Architecture | Encoder-only | Decoder-only |
| Attention | Bidirectional | Unidirectional |
| Pre-training | MLM + NSP | Next Token Prediction |
| Use Case | Understanding | Generation |

- 📓 **基础对比**：简单代码展示 BERT/GPT-2 模型原理
- 📊 **GLUE 评测**：标准化基准测试对比两者性能
- 🛠️ **本地部署**：完整演示模型下载与推理流程

## Project Structure | 项目结构

```
├── bert_gpt2.ipynb          # Basic BERT vs GPT-2 comparison
├── bert_gpt2_GLUE.ipynb     # GLUE benchmark evaluation
├── LICENSE
└── README.md
```

## Contributing | 贡献指南

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

> 💡 **Tip**: Ensure you have access to Hugging Face credentials before running the notebooks. GPU is recommended for model inference.
