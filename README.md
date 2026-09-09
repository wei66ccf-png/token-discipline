# token-discipline

用于 Codex 等支持 `SKILL.md` 的助手，减少重复读取、冗长工具输出、无效轮询和排版返工，同时保持完整交付与必要验证。

## 使用

将本仓库中的 `SKILL.md` 与 `references/` 放入个人技能目录下的 `token-discipline/`。Codex 默认位置为 `~/.codex/skills/token-discipline/`；设置了 `CODEX_HOME` 时使用其 `skills` 子目录。不要覆盖已有修改而不做比较。

在任务中明确调用：

```text
使用 $token-discipline 完成这个任务，保持交付完整和必要验证。
```

也可由支持技能发现的平台按任务选择。它是一套执行规则，不是硬性token计费器，也不保证每轮自动加载。无需额外运行时依赖。

## 主要规则

- 浏览只取必要内容，实际处理数据保持完整。
- 环境依赖一次探测，系统性失败停止同类重试。
- 等待采用完成事件或合理退避。
- 先验证代表性页面，再复制样式；修复只检查受影响部分。
- 全部范围完成且必要检查通过后立即交付。

## 目录

- [SKILL.md](SKILL.md)：日常执行入口。
- [文件工作流](references/file-workflows.md)：文档、PPT等任务按需读取。
- [评估方法](references/evaluation.md)：行为核对与前后对照方法。
- [研究记录](references/research.md)：参考的GitHub项目与取舍。

本项目尚未进行配对token成本基准测试，不宣传未经验证的节省比例。研究记录中的第三方成果不代表本项目效果。