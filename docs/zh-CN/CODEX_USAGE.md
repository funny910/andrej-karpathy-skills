# 在 Codex 中使用 Karpathy Guidelines

在 Codex 中可直接调用：

```text
$karpathy-guidelines
```

适合以下任务：

- 开始编码前澄清假设和成功标准
- 控制改动范围，避免顺手重构
- 审查是否存在过度设计
- 为修复建立最小可验证检查

示例：

```text
用 $karpathy-guidelines 审查这次修改，指出无关变更和过度抽象，
并给出最小验证命令。
```

## 使用边界

- Fork 的 `main` 用于上游同步。
- Codex 的全局 skill 安装与这个 GitHub Fork 是两件事。
- 项目专属规则放在项目自己的 `AGENTS.md` 或其他已批准配置中。
- 不要把这套准则无差别追加到所有项目的根指令文件。
