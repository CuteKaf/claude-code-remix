# Claude Code Remix

一个面向 **结构研究、架构导读和后续改造** 的仓库。

这个仓库目前不是一个“已经完成魔改”的项目，而是一个建立在 Claude Code 源码快照之上的 **研究导览版工作区**。它的目标不是简单存档，而是帮助后续阅读、理解、拆解和定向改造。

---

## 这个仓库现在是什么

你可以把它理解成：

- 一个独立于原始仓库的公开研究仓库
- 一个以 TypeScript 快照为基础的阅读与分析入口
- 一个后续可以继续加入导读、结构图、模块分析和改造实验的公开工作区

它当前最适合做三件事：

1. **研究 Claude Code 的整体结构**
2. **建立阅读入口和模块导览**
3. **作为后续公开改造的起点**

---

## 当前状态判断

这个仓库现在仍然保留着一份大体量的 TypeScript 源码快照结构，因此：

- **适合研究**
- **适合做文档化导读**
- **不适合一上来就乱改代码**

更准确地说，它现在更像一个：

## **大型 agent / coding agent 源码研究仓库**

而不是一个已经清晰收敛目标的二开产品。

---

## 建议阅读顺序

如果你第一次研究这个仓库，建议优先看：

1. `docs/repo-overview.md`
2. `docs/how-to-read-this-repo.md`
3. `docs/upstream-update-summary-2026-03-31.md`
4. `docs/mirror-vs-remix-vs-upstream.md`

然后再进入源码：

1. `src/main.tsx`
2. `src/commands.ts`
3. `src/tools.ts`
4. `src/QueryEngine.ts`

---

## 仓库文档

### 导览与报告
- [`docs/repo-overview.md`](docs/repo-overview.md)
- [`docs/how-to-read-this-repo.md`](docs/how-to-read-this-repo.md)
- [`docs/upstream-update-summary-2026-03-31.md`](docs/upstream-update-summary-2026-03-31.md)
- [`docs/mirror-vs-remix-vs-upstream.md`](docs/mirror-vs-remix-vs-upstream.md)

### 备份内容
- [`docs/original-snapshot-readme.md`](docs/original-snapshot-readme.md)

---

## 当前结论

这个仓库最有价值的地方，不是“它已经改好了”，而是：

- 你已经有一个可以公开整理的研究仓库
- 你不需要在私有镜像上冒险动手
- 你可以先从阅读地图和结构理解开始
- 再逐步决定后面要不要做真正的公开魔改

---

## 下一步最适合做什么

如果继续往前推进，最值得做的是：

1. 给核心模块做分层导览
2. 拆解 Tool system
3. 拆解 QueryEngine 主循环
4. 拆解 command surface
5. 再决定是否进入代码级改造
