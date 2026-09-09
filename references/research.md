# 相似项目与优化取舍

检索与阅读日期：2026-09-09。以下内容是对公开项目的参考整理，采用自己的表述；未运行其安装脚本，也未复制其代码。

| 项目 | 阅读材料 | 采用的思路 | 未照搬的内容 |
|---|---|---|---|
| [token-diet](https://github.com/Kulaxyz/token-diet) | README | 定向读取、输出增量、按影响范围测试 | 固定测试数量上限、擅自选择便宜模型、极端电报体 |
| [benjamin-plus-skill](https://github.com/JetBrains/benjamin-plus-skill) | README、RULESET.md | 区分浏览与完整数据处理、批量环境探测、减少轮询 | 自动注入全局配置、无条件安装依赖、固定两句交付限制 |
| [Agent Skills for Context Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering) | README、context-optimization/SKILL.md相关部分 | 渐进加载、保留可取回证据、按实际收益决定上下文拆分 | 固定缓存收益比例、无法控制的宿主缓存操作、无授权自动委派 |

这些项目公布的节省数字与特定模型、任务、基线和计量方式有关。本技能尚未完成配对基准测试，不宣称固定节省比例或已经证明质量不变。

本次优化把高频规则放在短入口，把文件排版、评估和来源放在按需参考中；另外补充系统性错误时停止同类批处理，避免短输出掩盖失败。