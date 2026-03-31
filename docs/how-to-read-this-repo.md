# 这个仓库怎么读

## 推荐阅读顺序

### 第一步：看 4 个总入口
1. `README.md`
2. `src/main.tsx`
3. `src/commands.ts`
4. `src/tools.ts`
5. `src/QueryEngine.ts`

这一步的目标不是细读，而是先知道：
- 它怎么启动
- 有哪些命令
- 有哪些工具
- 主循环大概长什么样

---

## 第二步：选一个方向深挖

### 路线 A：Tool system
读：
- `src/tools.ts`
- `src/Tool.ts`
- `src/tools/`

### 路线 B：Command system
读：
- `src/commands.ts`
- `src/commands/`

### 路线 C：Query / context / memory
读：
- `src/QueryEngine.ts`
- `src/query/`
- `src/context*`
- `src/memdir/`
- `src/state/`

---

## 第三步：暂时不要优先碰的地方

如果你是第一次研究，建议后看：
- `bridge/`
- `remote/`
- `voice/`
- `vim/`
- `buddy/`
- `server/`

原因不是这些不重要，而是它们更偏外围增强层。

---

## 阅读目标应该是什么

第一次读，不要追求“把整个仓库都看懂”。
你更应该先回答这几个问题：

1. 这个程序从哪里启动
2. 命令入口怎么组织
3. 工具调用系统怎么组织
4. Query loop 在哪一层
5. 哪些模块是主干，哪些是附加层

只要这几个问题建立起来，这个仓库就不会再显得一团乱。
