# outcome-acceptance · 输入到结果验收

一个 Codex 技能。从原始诉求追到可观察的结果，用反例检验关键边界，再按实际证据报告已验证、失败和未验证的范围。

适用于代码改动、资料分析、自动化和外部系统集成。小改动可以直接检查结果及关键边界，复杂任务可采用场景表和独立复核。

## 安装

如果你的 Codex 环境带有 `skill-installer`，可以让 Codex 从本仓库安装技能。技能位于仓库根目录。也可以运行下面的命令。

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo HelloYoung2025/outcome-acceptance --path . --name outcome-acceptance
```

如果环境没有安装工具，可克隆本仓库，将 `SKILL.md`、`agents/`、`assets/` 和 `references/` 复制到自己的 Codex 技能目录下的 `outcome-acceptance/`。安装后重新启动 Codex 以加载技能。

## 使用

```text
使用 $outcome-acceptance 验收这项工作。先列出必须交付的结果和关键反例，再从真实入口核对到接收端，报告证据、未验证范围和阻断项。
```

- [技能入口](SKILL.md)
- [场景表、反例及核验细目](references/templates.md)
- [可复制的项目指令](assets/project-instruction.md)

[MIT License](LICENSE)
