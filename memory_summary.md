## User Profile

当前仅能确认该用户在使用本地文件式 agent memory 工作流，并要求用中文响应。现有 Phase 2 输入里没有任何 rollout 任务内容，因此没有足够证据总结更具体的长期工作偏好、项目背景或常用仓库。

## User preferences

- 默认使用中文响应。
- 当 memory 证据为空时，保留最小必需产物，不编造用户偏好、项目知识或验证结果。

## General Tips

- 在 `C:\Users\18235275112_120007\.codex\memories` 下运行 Phase 2 时，先读 `phase2_workspace_diff.md` 判断是 INIT 还是增量更新。
- 如果存在 `extensions/<name>/instructions.md`，必须先读取；只有扩展里的实际资源文件内容才能作为记忆证据，说明文件本身不是业务事实。[ad-hoc note]
- 当 `raw_memories.md` 只有 `No raw memories yet.` 且 `rollout_summaries/` 为空时，输出最小 `MEMORY.md` 和 `memory_summary.md` 即可，避免无意义 churn。

## What's in Memory

### C:\Users\18235275112_120007\.codex\memories

#### 2026-05-21

- memory-folder initialization / empty evidence state: raw_memories.md, No raw memories yet, phase2_workspace_diff.md, extensions/ad_hoc/instructions.md
  - desc: 记录该 memory 仓库第一次 Phase 2 整理时没有任何 rollout summary、raw task block 或 ad-hoc note 资源可整合的状态；当未来代理想确认“为什么这里只有最小记忆文件”时先查这里。适用范围为 `cwd=C:\Users\18235275112_120007\.codex\memories`。
  - learnings: 当前只有空的 `raw_memories.md` 和 `ad_hoc` 扩展说明，没有实际 note 资源文件；因此应保持最小初始化产物，而不是推断不存在的用户或项目记忆。[ad-hoc note]

### Older Memory Topics
