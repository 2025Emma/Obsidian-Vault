# Second Brain Coach

基于 Tiago Forte《Building a Second Brain》方法论的个人知识管理教练 Skill。

帮助你系统性地构建第二大脑：从 PARA 分类体系到 CODE 工作流程，从系统诊断到文件归档，把零散的信息变成可复用的知识资产。

## 功能

| 功能模块 | 说明 |
|---------|------|
| **系统诊断** | 评估当前知识管理系统的健康度，识别常见缺口，给出针对性改进建议 |
| **文件归档** | 遵循 PARA 四问决策树（项目/领域/资源/归档），引导你将文件归类到正确位置 |
| **实践问答** | 解答第二大脑实践中的具体问题，引用 BASB 核心概念和最佳实践 |

## 触发方式

在支持 Skill 的 Agent 中，直接提及以下关键词即可激活：

- "第二大脑"
- "PARA"
- "CODE"
- "文件归档"
- "知识管理"

## 安装方式

**通过 Agent 安装**

在 Claude Code、Codex、OpenClaw 等支持 Skill 的 Agent 中，直接对话：

```
安装这个 skill：https://github.com/2025Emma/second-brain-coach
```

**手动安装**

1. 克隆或下载本仓库
2. 将 `second-brain-coach/` 文件夹复制到你的 Agent Skills 目录：

| 工具 | 路径 |
|------|------|
| Claude Code | `~/.claude/skills/` |
| OpenClaw | `~/.openclaw/skills/` |
| Codex | `~/.codex/skills/` |
| WorkBuddy| `~/.workbuddy/skills/` |

3. 重启 Agent 或重新加载 Skills

## 仓库结构

```
second-brain-coach/
├── SKILL.md                     # Skill 定义：工作流、触发条件、约束规则
├── README.md                    # 本文件
├── LICENSE                      # MIT 许可证
└── references/                  # 知识库参考资料
    ├── basb-concepts.md         # BASB 核心概念、CODE 流程表、FAQ
    ├── para-decision-tree.md    # PARA 定义、四问决策脚本、示例
    ├── system-diagnosis-checklist.md  # 系统诊断问题清单、常见缺口
    └── practice-prompts.md      # Capture → Express 实践练习
```

## 使用说明

1. **激活 Skill**：提及第二大脑相关话题
2. **选择模式**：Agent 会询问你想进行【系统诊断】【文件归档】【实践问答】中的哪一项
3. **跟随引导**：根据所选模式，Skill 会引导你完成相应流程

### 引用规范

知识回答必须引用对应的参考文件章节，例如：
- `basb-concepts:承诺#2`
- `para-decision-tree:四问决策树`

## 验证

发布前可使用 skill-creator 验证工具检查：

```bash
python /path/to/skill-creator/scripts/quick_validate.py second-brain-coach
```

需要 `pyyaml`：
```bash
pip install pyyaml
```

## 关于参考资料

- 参考文件包含对 Tiago Forte 著作的原创性总结
- 避免大段引用原文，尊重版权
- 欢迎扩展 `references/` 添加自己的笔记，但请在 SKILL.md 中维护引用规范

## License

[MIT](./LICENSE)
