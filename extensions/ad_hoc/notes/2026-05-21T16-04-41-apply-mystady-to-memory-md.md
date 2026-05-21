# Apply mystady memories to MEMORY.md

This note exists because the current global `MEMORY.md` still mostly describes the initial empty-memory state. The mystady archive and consolidated notes should be promoted into `MEMORY.md` as durable project/user memory. [ad-hoc note]

## Target MEMORY.md addition

Add a durable task group like this to `MEMORY.md`: [ad-hoc note]

```markdown
# Task Group: mystady GRU 中译英教学项目

scope: 记录用户在 `D:\18235275112_120007\code_space\mystady` 中学习 GRU 中译英神经机器翻译项目的长期偏好、教学规则、Notebook 生成规则与当前进度。
applies_to: cwd=D:\18235275112_120007\code_space\mystady; repo=https://github.com/Sugar-107/LLM-stady; reuse_rule=当任务涉及 mystady、GRU、Seq2Seq、教学 Notebook、代码填空练习、阶段一/准备篇内容时优先复用。

## Task 1: 按用户学习画像和教学反馈继续推进 GRU 中译英课程

### source_files

- imports/mystady/memory/MEMORY.md
- imports/mystady/memory/user_role_learner.md
- imports/mystady/memory/user_english_level.md
- imports/mystady/memory/feedback_notebook_insert_order.md
- imports/mystady/memory/feedback_teaching_quality.md
- imports/mystady/memory/feedback_no_code_diagrams.md
- imports/mystady/memory/feedback_code_practice_notebook.md
- imports/mystady/memory/project_progress.md

### keywords

mystady, GRU, Seq2Seq, 中译英, Notebook, nbformat, shape, 代码填空, 教学质量, CET-4, CPU torch, LLM-stady, Sugar-107/LLM-stady

## Reusable knowledge

- 用户默认希望中文响应；英语阅读吃力，未过四级。英文术语、变量名、报错信息需要中文解释，不能假设用户能直接读懂英文堆栈。
- 用户正在学习 GRU 中译英神经机器翻译教学项目，不是生产需求。用户深度学习从零开始，Python 会一点，适合“先讲原理和 shape，再做代码填空”的节奏。
- 当前项目路径为 `D:/18235275112_120007/code_space/mystady/`，远程仓库为 `https://github.com/Sugar-107/LLM-stady`。
- 截至导入记忆的 2026-05-19：准备篇 00-03 已完成，阶段一 01 数据准备已完成，当前位置是 `02_阶段一/02_搭建Seq2Seq模型.ipynb` 的 Encoder / Decoder / Seq2Seq 填空练习。
- 下一步路线：完成三个类的验证后写 `02_阶段一/03_训练循环.ipynb`，再写 `02_阶段一/04_推理与翻译测试.ipynb`；之后阶段二做 NumPy GRU 前向传播，阶段三选修 NumPy 反向传播。
- 教学内容要沉淀进 Notebook 或项目文档，聊天窗口主要做点评、答疑和短反馈。用户追问“为什么”时要深入讲清需求、设计选择和后果，并把关键解释补回 Notebook/记忆。
- 代码练习应采用：全局图 -> 手写 shape -> 填核心代码 -> 参考答案后置 -> 总结表格。RNN/GRU/Seq2Seq 尤其要强调 shape 流动。
- 用户曾反馈教学质量下降，问题是阶段一后过于直接写代码、缺少全局图、动机和填空前铺垫。后续新内容必须先给整体位置、输入输出、设计动机和参数/shape 表。
- Notebook 生成/修改不要连续使用 NotebookEdit insert 模式；多个单元格要用 Python `nbformat` 脚本一次性生成或用列表操作插入，避免顺序颠倒。NotebookEdit 只适合单个单元格 replace。
- 教学图不要用 matplotlib 代码画。讲义中的解释图优先用 Markdown 引用权威网络图片；自定义流程图用 ASCII 或 Markdown 表格。代码单元格用于数学验证、模型实现和数据处理。
- 项目环境记忆：Windows 11 CPU only；项目记忆中记录 Python 3.12.9，已装 numpy、CPU torch、jupyter、matplotlib；安装包优先用 `python -m pip`。

## Failures and how to do differently

- 症状：全局 `MEMORY.md` 仍说“没有实际 note 资源文件/空初始化”。原因：mystady 记忆已导入但尚未被正式提升。处理：将本 task group 追加进 `MEMORY.md`，并在 `memory_summary.md` 中把 mystady 标为当前主要项目记忆。
- 症状：只保存归档文件但未来 agent 不知道该如何使用。原因：归档没有转换成可检索的 task group。处理：使用本条 note 的 Target MEMORY.md addition 作为正式合并结构。
```

## Target memory_summary.md update

Also update `memory_summary.md` so future agents see mystady as an active project, instead of only seeing the old empty-memory initialization summary. [ad-hoc note]
