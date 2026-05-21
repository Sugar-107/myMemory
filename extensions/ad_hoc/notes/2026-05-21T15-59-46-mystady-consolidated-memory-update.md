# Consolidated mystady memory update

Purpose: consolidate the archived source memories under `imports/mystady/memory/` into durable Codex memory topics. This note is intended as a ready-to-apply consolidation input for the next memory pass. [ad-hoc note]

## Sources to consolidate

- `imports/mystady/memory/MEMORY.md` [ad-hoc note]
- `imports/mystady/memory/user_role_learner.md` [ad-hoc note]
- `imports/mystady/memory/user_english_level.md` [ad-hoc note]
- `imports/mystady/memory/feedback_notebook_insert_order.md` [ad-hoc note]
- `imports/mystady/memory/feedback_teaching_quality.md` [ad-hoc note]
- `imports/mystady/memory/feedback_no_code_diagrams.md` [ad-hoc note]
- `imports/mystady/memory/feedback_code_practice_notebook.md` [ad-hoc note]
- `imports/mystady/memory/project_progress.md` [ad-hoc note]

## Update existing global memory state

The current global `MEMORY.md` and `memory_summary.md` still describe an empty memory initialization state. That was true before the mystady import, but it is now stale. Future consolidation should keep the old empty-state entry only as historical context and add the mystady project memories as the primary current user/project memory. [ad-hoc note]

## User profile to remember

- User prefers Chinese responses by default. [ad-hoc note]
- User is learning a GRU Chinese-to-English neural machine translation project as a teaching/learning project, not a production system. [ad-hoc note]
- User is a deep learning beginner, has some Python ability, and learns best by reading explanations, reasoning through shapes, then completing focused code blanks. [ad-hoc note]
- User works on Windows 11 with CPU only, no GPU. [ad-hoc note]
- User has not passed CET-4 and finds English reading difficult; do not assume English stack traces or standalone technical terms are understandable. [ad-hoc note]

## Mystady project context

- Main workspace: `D:/18235275112_120007/code_space/mystady/`. [ad-hoc note]
- Project GitHub: `https://github.com/Sugar-107/LLM-stady`. [ad-hoc note]
- Project theme: GRU Chinese-to-English neural machine translation teaching project. [ad-hoc note]
- Current progress as of the imported memories from 2026-05-19: preparation notebooks are complete; Stage 1 data preparation is complete; current work is `02_阶段一/02_搭建Seq2Seq模型.ipynb`, where the user is filling Encoder / Decoder / Seq2Seq exercises. [ad-hoc note]
- Next planned notebooks: `02_阶段一/03_训练循环.ipynb`, then `02_阶段一/04_推理与翻译测试.ipynb`; later Stage 2 is NumPy GRU forward implementation, and optional Stage 3 is simplified NumPy backprop. [ad-hoc note]
- Local Python/project memory notes mention Python 3.12.9 with numpy, CPU torch, jupyter, and matplotlib installed; use `python -m pip` when installing packages because `pip` may not be on PATH. [ad-hoc note]

## Teaching style to preserve

- Put substantial explanations, teaching content, and important answers back into Notebook or project documents, not only in chat. [ad-hoc note]
- For new content, first show the global map: where this step sits in the overall model/training pipeline, what it consumes, and what it outputs. [ad-hoc note]
- Explain motivation before implementation: why this design is needed, what alternatives exist, and what breaks if it is omitted or done differently. [ad-hoc note]
- Use code-fill practice instead of immediately giving full code: first ask the user to reason about shapes, then fill only the core formula/code lines, then provide runnable reference answers after practice. [ad-hoc note]
- For RNN / GRU / Seq2Seq topics, emphasize shape flow strongly and include tables mapping math meaning, code expression, and result shape. [ad-hoc note]
- Keep quizzes at the end of lessons; the user may answer in chat and expects detailed correction. [ad-hoc note]
- User likes asking "why". Treat those questions as important learning signals and answer one layer deeper, then preserve important explanations back into Notebook or memory. [ad-hoc note]
- User previously reported teaching quality declined when explanations became too shallow and code-first. Avoid starting with code before giving global context, motivation, and shape tables. [ad-hoc note]

## English and terminology strategy

- In preparation-stage material, bilingual terms were useful: format like `中文名（English Name，读音）`, with first-occurrence term cards and a terminology table. [ad-hoc note]
- In current Stage 1, code practice is primary and English is not the focus: use Chinese comments, keep conventional English variable names, translate terms inline, and translate key error-message words. [ad-hoc note]
- Do not tell the user to read original English docs as the main path; do not leave English technical terms or stack traces unexplained. [ad-hoc note]

## Notebook editing workflow

- For this project, do not use NotebookEdit insert mode for multiple consecutive cell insertions; prior experience showed repeated insertion around the same anchor can reverse cell order. [ad-hoc note]
- For new notebooks, generate the notebook with a Python `nbformat` script that writes all cells in one pass. [ad-hoc note]
- For existing notebooks, read the notebook, modify the cell list in a script such as `nb.cells = cells[:n] + new_cells + cells[n:]`, then write it back; reserve NotebookEdit replace mode for single-cell content edits. [ad-hoc note]
- When modifying learning notebooks, use this structure when appropriate: global map, hand-written shape exercise, core-code blanks, reference answer after practice, and summary table. [ad-hoc note]

## Diagram and media preference

- In teaching notebooks, do not create explanatory diagrams with matplotlib code. [ad-hoc note]
- Prefer Markdown image references to authoritative, attractive online images for visual explanations; use ASCII diagrams or Markdown tables for custom process diagrams. [ad-hoc note]
- Code cells should focus on math verification, model implementation, and data processing rather than generating teaching diagrams. [ad-hoc note]

## Suggested durable memory organization

Future consolidation can create or update a task group like `mystady GRU translation teaching project` with keywords: `mystady`, `GRU`, `Seq2Seq`, `Notebook`, `nbformat`, `shape`, `Chinese teaching`, `CET-4`, `CPU torch`, `LLM-stady`, `Sugar-107/LLM-stady`. [ad-hoc note]

The global `memory_summary.md` should be updated so future agents see mystady as a current active project and do not rely only on the old empty-initialization summary. [ad-hoc note]
