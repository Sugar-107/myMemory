---
name: 学习者画像
description: 用户在学 GRU 中译英翻译项目，深度学习零基础，Python 初级，已完成准备篇全部内容，正在阶段一搭建 Seq2Seq 模型
type: user
originSessionId: da78c696-22fe-45e2-ab9e-53a58a7bfdbb
---
用户正在学习 **GRU 中译英神经机器翻译项目**（教学项目，不是生产需求）。

## 学习者画像

- **编程**：Python 会一点，能看懂代码，动手能力在练习中
- **深度学习**：从零基础开始，已学完准备篇（矩阵乘法、梯度、神经网络）
- **数学**：经过学习已能理解梯度下降、链式法则、GRU 公式推导
- **硬件**：Windows 11 + CPU only，无 GPU
- **英语**：没过四级（详见 user_english_level.md）

## 当前进度（2026-05-19）

```
✅ 准备篇 00：矩阵乘法直觉
✅ 准备篇 01：梯度与链式法则
✅ 准备篇 02：神经网络的三件事
✅ 番外篇：GRU 公式推导（RNN → GRU 完整推导）
✅ 阶段一 01：数据准备（语料、词表、Dataset、DataLoader）
⏳ 阶段一 02：搭建 Seq2Seq 模型（Encoder + Decoder 填空练习中）
⬜ 阶段一 03：训练循环
⬜ 阶段一 04：推理与翻译测试
⬜ 阶段二：NumPy 实现 GRU 前向传播
⬜ 阶段三（选修）：NumPy 手写反向传播
```

## 教学路径（已和用户对齐）

1. **阶段零/准备篇**：矩阵乘法 + 梯度/链式法则 + 神经网络基础 + GRU 公式推导
2. **阶段一**：用 PyTorch 跑通中译英 Seq2Seq（先看到"活"的翻译）
3. **阶段二**：用 NumPy 手写 GRU 前向传播，和 PyTorch 对齐验证
4. **阶段三（选修）**：NumPy 手写反向传播（用简化任务，不用真实翻译）

## 项目文件结构（2026-05-19 整理后）

GitHub：https://github.com/Sugar-107/LLM-stady

```
D:/18235275112_120007/code_space/mystady/
├── README.md
├── 教学计划.md
├── 01_准备篇/
│   ├── 00_矩阵乘法直觉.ipynb
│   ├── 01_梯度与链式法则.ipynb
│   ├── 02_神经网络的三件事.ipynb
│   └── 03_GRU公式推导.ipynb
└── 02_阶段一/
    ├── 01_数据准备.ipynb
    └── 02_搭建Seq2Seq模型.ipynb
```

## 讲解偏好（已验证有效）

- **所有讲解写进 Notebook**：用户明确要求"所有教学和讲解内容都写入 ipynb"，聊天窗口只做点评、答疑
- **代码训练为主**：用户说"注重代码"是指"讲清原理后让我自己写代码"，不是减少讲解
- **代码框架填空**：给代码框架让用户填空（⭐填空 → ⭐⭐提示 → ⭐⭐⭐独立），不直接给完整代码
- **Notebook 生成方式**：一律用 Python 脚本（nbformat）生成，不用 NotebookEdit 的 insert 模式（会乱序）

## 教学节奏

- 用户喜欢追问"为什么"——**鼓励这种追问**，每个追问都值得单独在 Notebook 里固化
- 用户会主动停下来问"这个符号理解不能"、"这个公式是怎么来的"——**不跳过，深度讲解**
- 每节课末尾有小测验，让用户用自己的话回答，写错是找盲点的工具
- 用户答完小测验后贴给我批改，我逐题点评

## 工具环境

- Python 3.12.9，已装：numpy 2.4.3、torch 2.10.0+cpu、jupyter 1.1.1、matplotlib
- IDE：IntelliJ IDEA Ultimate（遇到过 Jupyter session factory 问题，建议备用方案：直接用 Jupyter Lab）
- pip 命令要用 `python -m pip`（pip 不在 PATH）
- git 已配置，远程仓库：https://github.com/Sugar-107/LLM-stady
