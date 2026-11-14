# 安装 figure-aesthetics

## 通过 Codex 安装

在 Codex 中发送：

```text
使用 $skill-installer 安装 https://github.com/ZhimingYe/figure-aesthetics 中的技能，SKILL.md 位于仓库根目录。
```

## 手动安装

需要已安装 Git。以下两种安装范围选择一种即可。

### 所有项目可用

在终端执行：

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/ZhimingYe/figure-aesthetics.git ~/.agents/skills/figure-aesthetics
```

### 仅当前项目可用

在目标项目根目录执行：

```bash
mkdir -p .agents/skills
git clone https://github.com/ZhimingYe/figure-aesthetics.git .agents/skills/figure-aesthetics
```

安装后，确认技能目录中包含 `SKILL.md`、`references/` 和 `agents/`，不要只复制 `SKILL.md`。若目录中已有同名技能，保留原有修改，避免重复安装。

## 调用

在 Codex 中输入：

```text
使用 $figure-aesthetics 设计或优化这张科研图，以学术创意实现高级感、高信息密度与非海报感。
```

Codex 会自动发现技能；若未出现，请重启 Codex。也可在 Codex CLI 或 IDE 扩展中通过 `/skills` 查找。

## 更新

通过 Git 手动安装且没有本地修改时，执行与安装范围对应的命令：

```bash
# 所有项目可用的安装
git -C ~/.agents/skills/figure-aesthetics pull --ff-only

# 仅当前项目的安装：在项目根目录执行
git -C .agents/skills/figure-aesthetics pull --ff-only
```

技能目录和发现方式见 [OpenAI 官方技能文档](https://learn.chatgpt.com/docs/build-skills)。
