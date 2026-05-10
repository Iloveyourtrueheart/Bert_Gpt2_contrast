# BERT-GPT2 Contrast

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-EE4C2C.svg?style=flat&logo=pytorch)](https://pytorch.org/)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Transformers-FFD21E.svg?style=flat&logo=huggingface)](https://huggingface.co/)
[![arXiv](https://img.shields.io/badge/arXiv-cs.LG-b31b1b.svg)](https://arxiv.org/abs/1810.04805)

## 📖 项目描述 | Project Description

> 本项目系统性地对比 **BERT**（双向编码器）与 **GPT-2**（单向解码器）两种 Transformer 架构的核心差异，涵盖预训练目标设计、注意力机制对比以及下游任务性能评估。

一个专注于 **BERT** 与 **GPT-2** Transformer 架构深度对比的实践项目。通过直观的代码示例和标准化的 GLUE 基准评测，展示双向编码器与单向解码器在模型设计理念上的本质区别。

## 🚀 快速开始 | Quick Start

### 环境准备

```bash
# 克隆项目
git clone https://github.com/your-repo/bert-gpt2-contrast.git
cd bert-gpt2-contrast

# 创建虚拟环境（推荐）
python -m venv venv
source venv/bin/activate  # Linux/Mac
# 或 venv\Scripts\activate  # Windows
```

### 安装依赖

```bash
pip install torch>=2.0.0 transformers>=4.30.0 datasets>=2.14.0 notebook
```

### 运行项目

```bash
# 启动 Jupyter Notebook
jupyter notebook

# 依次打开并运行：
# 1. bert_gpt2.ipynb      → 基础架构对比
# 2. bert_gpt2_GLUE.ipynb → GLUE 基准评测
```

## ✨ 核心特性 | Features

| 特性 | 描述 |
|------|------|
| 🔬 **架构对比** | 深入解析 Encoder-only vs Decoder-only 设计理念 |
| 🧠 **注意力机制** | 双向注意力 vs 单向注意力的实现差异 |
| 📊 **预训练目标** | MLM+NSP vs Next Token Prediction 对比 |
| 🏆 **GLUE 评测** | 标准化自然语言理解基准测试 |
| 💻 **交互式 Notebook** | Jupyter 环境下的完整代码示例 |

## 📁 项目结构 | Project Structure

```
bert-gpt2-contrast/
├── bert_gpt2.ipynb          # BERT 与 GPT-2 基础对比演示
├── bert_gpt2_GLUE.ipynb     # GLUE 基准评测实验
├── LICENSE                  # MIT License
└── README.md                # 项目说明文档
```

## 🔍 BERT vs GPT-2 对比概览

| 特性 | BERT | GPT-2 |
|:----:|:----:|:-----:|
| **架构类型** | Encoder-only | Decoder-only |
| **注意力机制** | 双向自注意力 | 单向自注意力 |
| **预训练目标** | MLM + NSP | Next Token Prediction |
| **适用场景** | 理解任务 | 生成任务 |
| **典型应用** | 文本分类、问答、NER | 文本续写、对话、翻译 |
| **代表模型** | BERT-base, BERT-large | GPT-2-small, GPT-2-medium |

## 🤝 贡献指南 | Contributing

欢迎提交 Issue 和 Pull Request！

1. **Fork** 本仓库
2. 创建特性分支：`git checkout -b feature/your-feature-name`
3. 提交更改：`git commit -m 'Add some amazing feature'`
4. 推送分支：`git push origin feature/your-feature-name`
5. 提交 Pull Request

## 📚 相关资源 | Resources

- [BERT 原始论文](https://arxiv.org/abs/1810.04805)
- [GPT-2 原始论文](https://arxiv.org/abs/1909.05858)
- [Hugging Face Transformers](https://huggingface.co/transformers/)
- [GLUE Benchmark](https://gluebenchmark.com/)

## ⚠️ 注意事项

> 💡 **提示**
> - 运行本项目需要 GPU 支持以获得合理的推理速度
> - 请确保已配置 Hugging Face 访问权限
> - 首次运行时会自动下载模型，请保持网络连接

---

*Made with ❤️ for NLP enthusiasts*