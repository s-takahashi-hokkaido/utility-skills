# utility-skills

自作した Claude Code / Claude 向けスキルを集めておくリポジトリ。

## 構成

```
skills/
  <skill-name>/
    SKILL.md        # スキル本体（フロントマター + 手順）
    references/     # 任意: 詳細ドキュメント（必要時のみ読み込む）
    scripts/        # 任意: スキルから実行するスクリプト
```

## SKILL.md の書き方

先頭に YAML フロントマターを置く。`description` はスキルが呼ばれるかどうかを決める
一番重要な部分なので、「何をするか」と「いつ使うか」を具体的に書く。

```markdown
---
name: skill-name
description: 何をするスキルか。どんな場面・キーワードで使うか。
---

# Skill Name

## 手順
1. ...
```

## 使い方

個人用として使う場合は、リポジトリを clone して `~/.claude/skills/` からシンボリックリンクを張る。

```bash
git clone https://github.com/s-takahashi-hokkaido/utility-skills.git
ln -s "$PWD/utility-skills/skills/<skill-name>" ~/.claude/skills/<skill-name>
```

プロジェクト単位で使う場合は `.claude/skills/` 配下に置く。

## スキル一覧

| スキル | 概要 |
| --- | --- |
| （未作成） | |
