# mirror / remix / upstream 的关系

## 1. upstream：`instructkr/claude-code`
现在已经转向：
- Python-first porting workspace
- 不再以原始 TS 快照为主跟踪状态

适合：
- 关注作者当前方向
- 看 Python 重写/移植思路

---

## 2. mirror：`claude-code-mirror`
这是你的私有镜像。

特点：
- 保留旧的 TypeScript 快照状态
- 尽量少动
- 用于归档和结构研究

适合：
- 保真存档
- 回看旧结构
- 对比上游重构前后的差异

---

## 3. remix：`claude-code-remix`
这是你的公开研究/改造工作区。

特点：
- 可以公开整理
- 可以加入导览、报告、阅读地图
- 可以作为后续魔改起点

适合：
- 公开研究
- 文档化导读
- 后续结构化改造

---

## 建议分工

### mirror
- 不轻易动代码
- 保持旧快照价值

### remix
- 先加文档
- 先建阅读框架
- 后面再决定是否开始大规模改造

### upstream
- 只作为观察和对照对象
- 不建议直接当作你的研究主仓库
