# 仓库总览报告

## 一句话结论
`claude-code-remix` 目前不是一个已经完成改造的项目，而是一份 **具有很强研究价值的大型 agent 源码工作区**。

它当前最适合的用途是：
- 结构研究
- 架构导读
- 模块拆解
- 后续公开改造准备

---

## 仓库表面结构

当前顶层非常简单：

```text
.
├── README.md
└── src/
```

所以这个仓库的难点不在顶层，而在：

## `src/` 非常大、非常深、非常工程化。

---

## 核心模块概览

### 1. `src/main.tsx`
程序主入口，负责启动、初始化、配置、上下文、交互和命令装配。

### 2. `src/commands.ts` + `src/commands/`
命令系统。表明这个仓库不是单一命令工具，而是一个命令面很宽的 CLI agent 产品。

### 3. `src/tools.ts` + `src/tools/`
工具系统。是整个仓库最值得优先研究的层之一。

### 4. `src/QueryEngine.ts`
主循环 / agent orchestration 核心层。理解整个系统“怎么想、怎么调工具、怎么组织消息”时非常关键。

### 5. `src/services/`
服务整合层，包括 API、OAuth、MCP、LSP、plugins、memory 等。

### 6. `src/components/` / `src/screens/` / `src/ink/`
终端 UI 层。说明这是一个 React + Ink 的富终端应用，而不是简单脚本集合。

---

## 当前最值得研究的方向

### 方向 A：Tool system
适合研究 agent 能力边界。

### 方向 B：Query engine
适合研究主循环和工具调用流程。

### 方向 C：Command surface
适合研究产品功能面和入口设计。

---

## 当前不建议一开始就重度投入的方向

- `bridge/`
- `remote/`
- `voice/`
- `vim/`
- `buddy/`
- `server/`

这些模块可能很有趣，但不适合第一阶段阅读。

---

## 最实际的建议

如果你现在开始研究这个仓库，不要先改代码。
先做：

1. 建立阅读地图
2. 确定优先研究模块
3. 输出结构化笔记
4. 再考虑是否开始魔改
