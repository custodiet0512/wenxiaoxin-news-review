# 闻小新 · 写作、审核与校对助手

“闻小新”是面向新闻与新媒体内容的 Skill，也可按写作目的、读者和材料处理其他文本。它支持从参考文章提炼表达特点、根据事实材料写稿、审核事实与逻辑、校对文字、跨平台改编及修改后复审。闻新周报与校园资料仅在明确要求时作为可选参考。

## 直接从 GitHub 安装

仓库根目录就是完整的 Skill，`SKILL.md` 与 `references/`、`agents/`、`assets/` 等目录保持相对结构。Codex 可在终端运行：

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo custodiet0512/wenxiaoxin-news-review \
  --path . --name wenxiaoxin-news-review --method download
```

目标目录已存在时，安装脚本会停止，不会覆盖旧版本。安装后在新一轮对话中使用 `$wenxiaoxin-news-review`，或问“闻小新，你是谁，能做什么？”。这个命令已在隔离目录完成安装测试，取得全部规则文件并通过技能格式检查。个别 Python 环境若缺少可信 CA 证书，需要先修复其证书配置；本机测试使用了已安装的证书包。

也可以直接克隆仓库到宿主的技能发现目录；OpenClaw 的发现目录以自己的配置为准。若只需下载包，可取[完整 ZIP](wenxiaoxin-news-review.zip)，解压后放入技能目录。

## 使用与边界

可提供选题、参考文章、事实材料或现有稿件。闻小新会区分已核实、冲突和待核信息；联网、附件读取与格式导出取决于运行环境。技能不会自行增加宿主权限，不自动覆盖原稿或发布内容。

本仓库未选择开源许可证；参考材料的归属与改编范围见 [SOURCES.md](SOURCES.md)。现有验证不等于全部场景已在 Codex/OpenClaw 应用内测试。
