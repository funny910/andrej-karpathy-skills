# Karpathy Guidelines Fork 维护工作流

这个 Fork 用于维护编程准则的中文说明和 Codex 使用边界。

## 分支职责

- `main`：只跟踪 `multica-ai/andrej-karpathy-skills` 上游。
- `codex-custom`：保存中文说明和本地 Agent 使用约定。
- `feature/*`：一次具体的文档或规则实验。

不要直接修改上游的 `CLAUDE.md`、`CURSOR.md` 或核心 skill 文件来承载个人项目规则；项目规则应留在项目自己的配置文件中。

## 同步上游

```bash
git clone https://github.com/funny910/andrej-karpathy-skills.git
cd andrej-karpathy-skills
git remote add upstream https://github.com/multica-ai/andrej-karpathy-skills.git
git fetch upstream
git switch main
git merge --ff-only upstream/main
git push origin main
```

如果 `main` 有本地修改，先将修改移到 `codex-custom` 或 feature 分支，再同步上游。
