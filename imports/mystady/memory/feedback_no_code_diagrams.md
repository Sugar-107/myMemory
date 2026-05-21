---
name: 不用代码画图
description: 讲义里的图表用引用权威资源的方式展示，不用 matplotlib 代码生成
type: feedback
originSessionId: da78c696-22fe-45e2-ab9e-53a58a7bfdbb
---
**规则**：Notebook 讲义里需要展示图表时，**不要写 matplotlib 代码来画图**。

**Why**：用户明确说"不要写代码画图，记住"。代码画的图需要用户跑代码才能看到，而且图的质量不如权威资源的图美观。直接引用网络上权威且美观的图片更直接、更有冲击力。

**How to apply**：

1. **引用网络图片**：用 Markdown 的 `![说明](URL)` 语法直接嵌入图片
2. **优先使用的权威资源**：
   - RNN/GRU 动图：`https://cdn-images-1.readmedium.com/v2/resize:fit:800/1*lNNJOWnMjxLzdUnUQqwKcw.gif`（GRU）
   - RNN 动图：`https://cdn-images-1.readmedium.com/v2/resize:fit:800/1*xn5kA92_J5KLaKcP7BMRLA.gif`
   - GRU 结构图来源：`https://fengchao.pro/blog/gru/`
3. **需要定制流程图时**：用 ASCII 文字图或 Markdown 表格来说明，不用代码画
4. **代码单元格只用于**：数学验证、模型实现、数据处理——不用于生成图表
