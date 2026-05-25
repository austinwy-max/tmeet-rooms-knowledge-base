# 腾讯会议 Rooms 问题排障知识库

> 从 IMA 知识库自动同步，每周一更新。

## 目录结构

- `notes/` — 笔记原文（Markdown 格式，14 篇）
- `files/` — 小文件（图片、PDF 等，<100MB）
- `manifest.json` — 知识库索引（包含所有条目的元数据）
- **大文件**（如 177MB 的产品培训 PPT）以 [GitHub Release](https://github.com/austinwy-max/tmeet-rooms-knowledge-base/releases) 资产形式提供，详见 `manifest.json` 中 `storage: github_release` 的条目

## 内容说明

腾讯会议 Rooms 产品相关技术支持知识：
- Rooms 工单故障记录
- 客户端已修复问题
- 网络问题排查
- 音频问题排查
- 云录制功能
- Rooms 功能说明
- 通用问题（进退会、弹窗、UDP/QUIC 原理等）
- 产品培训材料（PPT，存于 Release）

## 使用方式

### 同事方（推荐）

安装 `rooms-kb-sync` skill，按提示完成 2 步：
1. `git clone https://github.com/austinwy-max/tmeet-rooms-knowledge-base.git ~/.workbuddy/knowledge-bases/tmeet-rooms-knowledge-base`
2. 设置每周一 9:30 自动 `git pull` + 写入 MEMORY.md

> Clone 仅约 100KB（不含大文件）。需要 PPT 时通过 manifest.json 中的 `download_url` 单独下载。

### 维护方（Yangwei）

由 `sync_kb_to_git.py` 脚本每周一自动从 IMA 知识库同步，自动 commit + push。

## 维护者

yangwei
