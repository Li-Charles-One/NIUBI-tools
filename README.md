# NIUBI Tools

精选 **实用工具清单**（CLI、MCP：代码检索、搜索增强、浏览器与桌面控制等）。

> 用法：当 **GitHub 清单** 看即可，日常不必 clone。  
> 需要某个工具时，点「上游」按官方文档安装到你的 Agent。  
> 与 [NIUBI-skills-collection](https://github.com/Li-Charles-One/NIUBI-skills-collection) 分工：那边是 Agent **Skill**；这边是 **工具本体**。

适配：Claude Code / Cursor / Codex / OpenCode 等。

## 工具列表

| 工具 | 类型 | 功能 | 上游 |
|------|------|------|------|
| codegraph | CLI + MCP | 本地代码知识图谱：符号 / 调用链一键探索 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) |
| exa-mcp-server | MCP | Exa 网页搜索 / 代码搜索 / 公司研究 | [exa-labs/exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) |
| playwright-mcp | MCP | 微软官方浏览器自动化：网页点击/填表/快照/截屏/会话保持 | [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) |
| Windows-MCP | MCP | Windows 桌面端系统控制：鼠标/键盘/应用启动/截屏/UI树识别 | [CursorTouch/Windows-MCP](https://github.com/CursorTouch/Windows-MCP) |

## 怎么用（使用者）

1. 在本页表格里挑工具  
2. 打开「上游」仓库，按官方 README 安装（MCP / CLI）  
3. 在你的 Agent 配置里启用后使用  

**不需要** 把本仓库 clone 到本地当依赖。

## 维护说明（维护者）

本仓用 **git submodule** 钉住上游 commit，方便对版本；不是给最终用户跑的。

```bash
git clone --recurse-submodules https://github.com/Li-Charles-One/NIUBI-tools.git
git submodule update --remote --merge   # 同步上游
```

```
NIUBI-tools/
└── tools/
    ├── codegraph/              ← submodule
    ├── exa-mcp-server/         ← submodule
    ├── playwright-mcp/         ← submodule
    └── Windows-MCP/            ← submodule
```

## 收录原则

- 面向开发辅助、搜索检索、浏览器与桌面自动化等实用工具本体  
- 有独立上游 → 子模块跟踪；使用者仍去上游安装  
- 不是 Agent Skill（去 NIUBI-skills-collection）

## 贡献

欢迎 Issue / PR 推荐新工具或更新子模块指针。
