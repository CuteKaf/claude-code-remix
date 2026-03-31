# 上游更新摘要（2026-03-31）

## 一句话结论
上游 `instructkr/claude-code` 不是简单更新，而是一次方向性重构：

- 从 **TypeScript 源码快照仓库**
- 转向 **Python-first porting workspace**

---

## 上游新增了什么

### 1. 新 README
README 现在明确把仓库定位成：

`Claude Code Python Porting Workspace`

### 2. Python 主源码树
README 显示当前 `src/` 主要包含：
- `__init__.py`
- `commands.py`
- `main.py`
- `models.py`
- `port_manifest.py`
- `query_engine.py`
- `task.py`
- `tools.py`

### 3. `tests/`
新增了用于验证当前 Python workspace 的测试目录。

### 4. 新的 essay / 立场材料
新增文档：
- `2026-03-09-is-legal-the-same-as-legitimate-ai-reimplementation-and-the-erosion-of-copyleft.md`

### 5. `assets/omx/`
新增 OmX 工作流截图。

---

## 上游删除或放弃了什么

上游不再以原本那套大体量 TypeScript 快照为主 tracked state。

大量被移除或不再保留为主内容的包括：
- `QueryEngine.ts`
- `Task.ts`
- `Tool.ts`
- 大量 `bridge/`
- 大量 `cli/`
- 大量 `commands/*.ts`
- 大量外围增强模块

---

## 变化方向是什么

这次变化不是普通功能更新，
而是仓库身份的切换：

- 过去：快照研究仓库
- 现在：Python porting / rewrite workspace

---

## 对镜像意味着什么

你手里的私有镜像现在更有价值了。

因为它保留的是：
- 更新前的大体量 TypeScript 快照状态

而上游当前主仓库已经不再以那份 TS 树为主体。

所以：
- 私有镜像更适合归档与研究旧结构
- remix 更适合公开整理与后续导读
