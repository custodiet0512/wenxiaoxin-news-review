# 闻小新 · 写作、审核与校对助手

闻小新是一份面向写作、审核与校对的 Skill。它可以学习参考文本的表达特点，根据事实材料写新稿，也可以检查事实依据、逻辑与文字，并在修改后复审。新闻与新媒体是常见场景，文体不设固定清单；闻新周报相关建议仅在明确要求时使用。

## 主要功能

- 表达学习与写作：提炼范文的语气、用词和节奏，结合新材料成稿，不移植范文事实或引语。
- 事实与内容审核：核对来源、数据、标题、逻辑和待核信息，逐条给出依据与建议。
- 文字校对与改编：检查字词、数字、标点和一致性，按读者与平台调整表达。
- 修改后复审：对照旧问题，标出已解决、仍待处理和新增问题。

## 下载与安装

### Git Clone

```bash
git clone https://github.com/custodiet0512/wenxiaoxin-news-review.git
```

### ZIP 下载

[下载最新 main 分支 ZIP](https://github.com/custodiet0512/wenxiaoxin-news-review/archive/refs/heads/main.zip)

### 安装到 Agent

可安装技能就是仓库根目录 `wenxiaoxin-news-review/`。将这个**完整目录**复制到 Agent 使用的 skills 目录，不要只复制 `SKILL.md`。Codex 和 OpenClaw 的技能目录及刷新方式以各自配置为准；支持 `$skill-name` 语法的平台可调用 `$wenxiaoxin-news-review`。

仓库根目录已用 Git 克隆及 Codex 技能安装脚本分别在隔离目录测试，全部规则文件可用且格式校验通过。也可下载[单独的技能 ZIP](wenxiaoxin-news-review.zip)。

## 使用示例

```text
使用 $wenxiaoxin-news-review。学习下面两篇文章的语言表达，根据我提供的事实材料写一篇新稿，再审核事实、校对文字；不确定的信息请标出。
```

```text
使用 $wenxiaoxin-news-review。审校这篇文章，列出有依据的问题和修改建议，给出保留原意的修订稿。
```

安装后也可以问：“闻小新，你是谁？能做什么？”

## 目录

```text
wenxiaoxin-news-review/
├── SKILL.md
├── agents/openai.yaml
├── references/
├── assets/
├── examples/
└── tests/
```

## 使用边界

实际联网、附件读取和导出能力取决于宿主。技能不增加系统权限，不自动覆盖原稿、外传私稿或发布内容；待核稿不等于正式发布批准。来源与改编范围见 [SOURCES.md](SOURCES.md)。本仓库未选择开源许可证。
