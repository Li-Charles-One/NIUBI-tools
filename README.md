# NIUBI Search Tools

精选 **搜索 / 检索 / 上下文增强** 工具合集（CLI、MCP、索引器），以 Git 子模块方式组织，方便追踪上游更新。

> 与 [NIUBI-skills-collection](https://github.com/Li-Charles-One/NIUBI-skills-collection) 分工：那边放 Agent **Skill**；这边放 **工具本体**（不是 SKILL.md）。

适配：Claude Code / Cursor / Codex / OpenCode 等支持 MCP 或 CLI 的 Agent。

## 使用方法

克隆本仓库（含子模块）：

```bash
git clone --recurse-submodules https://github.com/Li-Charles-One/NIUBI-search-tools.git
```

已克隆但子模块为空？执行：

```bash
git submodule update --init --recursive
```

更新所有子模块到最新版本：

```bash
git submodule update --remote --merge
```

## 工具列表

| 工具 | 类型 | 功能 | 链接 |
|------|------|------|------|
| [codegraph](./tools/codegraph) | CLI + MCP | 本地代码知识图谱：符号 / 调用链一键探索，省 token | [原仓库](https://github.com/colbymchenry/codegraph) |
| [exa-mcp-server](./tools/exa-mcp-server) | MCP | Exa 网页搜索 / 代码搜索 / 公司研究 | [原仓库](https://github.com/exa-labs/exa-mcp-server) |
| [tavily-mcp](./tools/tavily-mcp) | MCP | Tavily 实时搜索 / 抽取 / 地图 / 爬取 | [原仓库](https://github.com/tavily-ai/tavily-mcp) |

### 计划收录（尚未子模块）

| 工具 | 类型 | 功能 |
|------|------|------|
| Context7 | MCP | 最新库文档 / API 示例检索 |
| Firecrawl | CLI + MCP | 网页搜索 / 抓取 / 爬取 |

## 目录结构

```
NIUBI-search-tools/
└── tools/
    ├── codegraph/        ← git submodule
    ├── exa-mcp-server/   ← git submodule
    └── tavily-mcp/       ← git submodule
```

## 收录原则

- 面向 **搜索、检索、文档、代码索引、上下文增强**
- 有独立上游仓库 → 用 **git submodule** 同步
- 不是 Agent Skill（那些去 NIUBI-skills-collection）

## 贡献

发现好用的搜索/检索工具？欢迎提 Issue 推荐或 PR 添加子模块。
