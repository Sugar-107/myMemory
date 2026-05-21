---
name: Notebook 生成规则
description: 生成和修改 Notebook 的正确方式，以及被用户指出的错误
type: feedback
originSessionId: da78c696-22fe-45e2-ab9e-53a58a7bfdbb
---
**规则**：向已有 Notebook 插入多个单元格时，**不要使用 NotebookEdit 的 insert 模式连续插入**。

**Why**：连续用同一个 cell_id 当锚点时，后插的单元格会排在前面，导致顺序颠倒。用户明确指出过："你每次添加 cell 的时候顺序不对"。

**How to apply**：

生成或修改 Notebook 的正确做法：

1. **新建 Notebook**：用 Python 脚本（nbformat）一次性写完所有单元格，用 `Write` 工具写入 `.py` 脚本，再用 `Bash` 运行它。这样顺序由代码决定，绝对正确。

2. **修改已有 Notebook（追加内容）**：
   - 用 `Read` 或 Bash 脚本读出当前所有单元格
   - 在 Python 脚本里用列表操作插入新内容（`nb.cells = cells[:n] + new_cells + cells[n:]`）
   - 用 `Write` 写脚本，`Bash` 运行

3. **NotebookEdit**：只用于单个单元格的内容修改（replace 模式），不用于 insert。

**关联项目**：D:\18235275112_120007\code_space\mystady\ 下所有 `.ipynb` 讲义。
