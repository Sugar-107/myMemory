# Import mystady project memory

Source directory: `D:\18235275112_120007\code_space\mystady\memory\`
Imported on: 2026-05-21
Purpose: merge project-local teaching/project memories into the global Codex memory workflow.

## Source files imported

- `MEMORY.md` — project-local memory index. [ad-hoc note]
- `user_role_learner.md` — learner profile and teaching path. [ad-hoc note]
- `user_english_level.md` — English level and terminology strategy. [ad-hoc note]
- `feedback_notebook_insert_order.md` — correct Notebook generation/editing workflow. [ad-hoc note]
- `feedback_teaching_quality.md` — teaching quality feedback and improvement rules. [ad-hoc note]
- `feedback_no_code_diagrams.md` — diagram/image preference for teaching notebooks. [ad-hoc note]
- `feedback_code_practice_notebook.md` — code-practice Notebook structure. [ad-hoc note]
- `project_progress.md` — current learning project progress. [ad-hoc note]

## User and project context

- User is learning a GRU Chinese-to-English neural machine translation teaching project, not a production system. [ad-hoc note]
- User is a beginner in deep learning, has some Python ability, learns by reading and completing code exercises, and works on Windows 11 CPU-only. [ad-hoc note]
- User prefers Chinese responses. English reading is difficult; user has not passed CET-4. [ad-hoc note]
- Project path is `D:/18235275112_120007/code_space/mystady/`; GitHub remote is `https://github.com/Sugar-107/LLM-stady`. [ad-hoc note]
- Python environment noted by the project memory: Python 3.12.9 with numpy, torch CPU, jupyter, and matplotlib available; use `python -m pip` because `pip` may not be on PATH. [ad-hoc note]

## Learning progress as of 2026-05-19

- Completed: preparation notebooks for matrix multiplication intuition, gradients/chain rule, neural-network basics, and GRU formula derivation. [ad-hoc note]
- Completed: Stage 1 data preparation notebook. [ad-hoc note]
- Current: Stage 1 `02_搭建Seq2Seq模型.ipynb`, filling in Encoder / Decoder / Seq2Seq code exercises. [ad-hoc note]
- Next: after those classes validate, create `03_训练循环.ipynb`, then `04_推理与翻译测试.ipynb`. [ad-hoc note]
- Later path: Stage 2 NumPy GRU forward implementation; optional Stage 3 NumPy backprop on a simplified task. [ad-hoc note]

## Teaching preferences

- Put all substantial teaching and explanations into Notebook or project documents, not only in chat. [ad-hoc note]
- User wants to write more code, but this means "explain the principle clearly, then let me fill/write code", not reducing explanation depth. [ad-hoc note]
- Use code frameworks with blanks: start with shape reasoning, then fill only the important core formula/code lines, then provide runnable reference answers after practice. [ad-hoc note]
- For RNN/GRU/Seq2Seq topics, emphasize shape flow strongly. [ad-hoc note]
- Each lesson should include a small quiz; user may answer in chat for detailed correction. [ad-hoc note]
- When the user asks "why", answer one layer deeper: explain the requirement, design choices, and consequences, then preserve important points back into Notebook or memory. [ad-hoc note]

## English and terminology strategy

- During the preparation phase, the user wanted bilingual terminology such as `中文名（English Name，读音）`, with first-occurrence term cards and a terminology table. [ad-hoc note]
- Current Stage 1 strategy: code is primary and English is not the focus; use Chinese comments, keep conventional English variable names, translate English terms inline, and translate key error-message words. [ad-hoc note]
- Do not assume the user can read English stack traces; do not leave English technical terms unexplained. [ad-hoc note]

## Notebook workflow and quality rules

- Do not use NotebookEdit insert mode for multiple consecutive cell insertions; it can reverse order when using the same anchor cell. [ad-hoc note]
- Generate new notebooks with a Python/nbformat script that writes all cells in one pass. [ad-hoc note]
- For existing notebooks, read cells, modify the cell list in a script, and write the notebook back; use NotebookEdit only for single-cell replacement. [ad-hoc note]
- Before code fill-in exercises, provide a global map, motivation, and a table of layers/parameters/forward input-output shapes. [ad-hoc note]
- User reported on 2026-05-19 that teaching quality had declined; avoid jumping straight into code without global context, motivation, and shape explanation. [ad-hoc note]

## Diagram/image preference

- In teaching notebooks, do not write matplotlib code just to draw explanatory diagrams. [ad-hoc note]
- Prefer Markdown image references to authoritative, attractive online resources; use ASCII diagrams or Markdown tables for custom process diagrams. [ad-hoc note]
- Code cells should be for math verification, model implementation, and data processing, not for generating teaching diagrams. [ad-hoc note]
