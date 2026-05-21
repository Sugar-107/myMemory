# Task Group: memory-folder initialization / empty evidence state

scope: 记录当前 memory 目录处于初始化阶段且暂无可整合任务证据时的最小状态；仅用于未来代理快速判断缺少 rollout 级记忆输入
applies_to: cwd=C:\Users\18235275112_120007\.codex\memories; reuse_rule=仅当该 memory 仓库仍缺少有效 raw memories、rollout summaries 与 ad-hoc note 资源时可直接复用，否则应以新增证据覆盖

## Task 1: 初始化 Phase 2 产物，确认当前没有可沉淀的任务记忆

### rollout_summary_files

- none available (cwd=C:\Users\18235275112_120007\.codex\memories, rollout_path=missing, updated_at=2026-05-21, thread_id=unknown, INIT run with empty `raw_memories.md`)

### keywords

- raw_memories.md, No raw memories yet, phase2_workspace_diff.md, INIT, empty evidence state, extensions/ad_hoc/instructions.md

## Reusable knowledge

- `phase2_workspace_diff.md` 显示本次仅新增了 `raw_memories.md`，其内容是 `No raw memories yet.`，因此当前没有 rollout 级证据可提升为 durable memory。
- `rollout_summaries/` 目录为空；未来若出现 `rollout_summaries/*.md`，应优先把它们与 `raw_memories.md` 中对应 task block 建立映射，再重写本块。
- `extensions/ad_hoc/instructions.md` 存在，但当前 `extensions/ad_hoc/` 下没有 note 资源文件，所以没有可整合的扩展来源信息。[ad-hoc note]

## Failures and how to do differently

- 症状：Phase 2 运行时只有空的 `raw_memories.md`，没有 rollout summary，也没有扩展 note 资源。原因：还没有经过可沉淀的 Phase 1 输出。处理：保留最小 `MEMORY.md` / `memory_summary.md`，不要编造任务组、用户偏好或流程知识。
- 症状：未来看到 `ad_hoc` 扩展存在就想当然写入记忆。原因：把扩展说明误当成 note 内容。处理：只有 `extensions/<name>/` 下实际 note 资源文件中的信息才能进入记忆；`instructions.md` 只定义解释规则，不提供业务事实。[ad-hoc note]
