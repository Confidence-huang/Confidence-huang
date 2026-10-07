# Confidence Huang

<p align="center">
  证据优先的系统 · Agent 技能 · 实用工作流软件
</p>

我做一些**小而可检查**的系统，把杂乱的工作变成明确的下一步：管住 AI Agent 行为的纪律与能力治理工具、
给研究成果和 Office 交付物把关的工作流、把视频变成可复习材料的学习管线，
以及把职业服务工作约束在明确边界内的软件。

## 从这里开始

| 你想做什么 | 从这里看起 |
| --- | --- |
| 让 AI Agent 的每次改动都留下可回退的点 | [`agent-git-discipline`](https://github.com/Confidence-huang/agent-git-discipline) |
| 在 Windows / Linux 上治理 Skill 与插件的生命周期 | [`skill-lifecycle-manager`](https://github.com/Confidence-huang/skill-lifecycle-manager) |
| 构建并验收研究报告或 Office 交付物 | [`academic-workstation`](https://github.com/Confidence-huang/academic-workstation) |
| 写一篇保留源文件的 LaTeX / Word 论文 | [`academic-paper-workflow`](https://github.com/Confidence-huang/academic-paper-workflow) |
| 产出并验收一份可编辑的 PPT | [`academic-ppt-workflow`](https://github.com/Confidence-huang/academic-ppt-workflow) |
| 把可访问的视频变成结构化中文笔记 | [`bilibili-douyin-video-learning`](https://github.com/Confidence-huang/bilibili-douyin-video-learning) |
| 把 B 站 / 抖音收藏归档进 Obsidian 知识库 | [`bilibili-vault-link`](https://github.com/Confidence-huang/bilibili-vault-link) · [`douyin-vault-link`](https://github.com/Confidence-huang/douyin-vault-link) |
| 让校园网开机自动登录（Windows，可审计） | [`AHU-Network-AutoConnect`](https://github.com/Confidence-huang/AHU-Network-AutoConnect) |
| 看一个职业服务产品从故事到服务边界 | [`careerpathdesk-website`](https://github.com/Confidence-huang/careerpathdesk-website) → [`careerpathdesk-frontend`](https://github.com/Confidence-huang/careerpathdesk-frontend) → [`careerpathdesk-backend`](https://github.com/Confidence-huang/careerpathdesk-backend) |

## 公开项目地图

### 一、Agent 纪律与能力治理

| 项目 | 它做什么 |
| --- | --- |
| [`agent-git-discipline`](https://github.com/Confidence-huang/agent-git-discipline) | 让 AI 编码 Agent 的**每次改动都留下可回退的点**，并把这条纪律机械地同步到多个 Agent、多个项目、多个平台。写给同时用 Codex / opencode / Claude Code / Cursor 的人：规则散在五处、改一处忘一处，最后一处都不可靠。 |
| [`skill-lifecycle-manager`](https://github.com/Confidence-huang/skill-lifecycle-manager) | 在 Windows 与 Linux 上治理 Skill 与插件的盘点、验证、安装、更新、备份与证据链；先看清现场，再动手改。 |

### 二、学术与 Office 工件工作流

| 项目 | 它做什么 |
| --- | --- |
| [`academic-workstation`](https://github.com/Confidence-huang/academic-workstation) | 共享的路由、结构检查、原生验收、PDF / 视觉 QA，以及证据与恢复契约。 |
| [`academic-paper-workflow`](https://github.com/Confidence-huang/academic-paper-workflow) | 把自然语言的论文请求路由到**保留源文件**的 LaTeX 或 Word 工作流，带引用、版式与视觉 QA 关卡。 |
| [`academic-ppt-workflow`](https://github.com/Confidence-huang/academic-ppt-workflow) | 把演示请求路由到**可编辑**的 PowerPoint 工作流，随后做原生往返与 PDF / 视觉验收。 |

它们共享的形状是：

```text
请求 → 路由 → 构建 → 结构检查 → 原生往返 → PDF/视觉 QA → 证据
```

### 三、视频 → 学习材料

内容侧一件技能、归档侧两个 Obsidian 插件，共用**同一套引擎**（一份实现、两个入口，因此永不漂移）：

| 项目 | 它做什么 |
| --- | --- |
| [`bilibili-douyin-video-learning`](https://github.com/Confidence-huang/bilibili-douyin-video-learning) | 把可访问的 B 站 / 抖音来源变成结构化中文笔记、复习材料、行动清单与 Anki 卡片，同时守住平台与隐私边界。 |
| [`bilibili-vault-link`](https://github.com/Confidence-huang/bilibili-vault-link) | Obsidian 伴生插件：粘贴 BV / av / b23 链接即归档；深度归档产出「关键帧 × 本地转写」图文对照笔记，逐帧配本机视觉模型图注。 |
| [`douyin-vault-link`](https://github.com/Confidence-huang/douyin-vault-link) | 同构的抖音版：收藏夹同步 + 单链接归档 + 本地 AI 分类 / 图文 OCR + 深度归档；自 v2.0.0 起删净云端 ASR 与云 AI 依赖。 |

```text
链接 / 收藏夹 → 取流(yt-dlp) → 场景打分自适应抽帧 → 本地 faster-whisper 转写
              → 时间对齐图文对照 → 本机 Ollama 逐帧图注 → 幂等笔记
```

### 四、校园网络

| 项目 | 它做什么 |
| --- | --- |
| [`AHU-Network-AutoConnect`](https://github.com/Confidence-huang/AHU-Network-AutoConnect) | 安徽大学校园网（Dr.COM eportal）自动登录：开机 / 插网线 / Wi-Fi 重连时静默完成认证。纯 PowerShell、无第三方依赖、无常驻进程、全程当前用户权限。事件驱动（用户登录 + NetworkProfile 事件 + 每小时保活三层兜底），能识别被 TUN / 代理虚拟网卡抢占的默认路由并回落物理接口，登录请求显式绕过系统代理，与代理软件互不干扰。 |

### 五、CareerPathDesk

从产品叙事到服务边界，切成三层清晰的公开面、用户面与服务面：

```text
website  →  frontend  →  backend
介绍与演示    角色工作台     权限、事务与审计证据
```

| 仓库 | 职责 |
| --- | --- |
| [`careerpathdesk-website`](https://github.com/Confidence-huang/careerpathdesk-website) | 产品故事与第一方演示入口。 |
| [`careerpathdesk-frontend`](https://github.com/Confidence-huang/careerpathdesk-frontend) | Vue 3 / TypeScript 的三角色工作台（老板端、老师端、学生端）。 |
| [`careerpathdesk-backend`](https://github.com/Confidence-huang/careerpathdesk-backend) | Go / PostgreSQL 服务边界：授权、事务与最小化审计证据。 |

## 共同线索

- **证据先于结论**：一个状态标签必须能指回一次可复现的检查。
- **边界显式**：凭据、隐私数据与生产动作留在公开示例之外。
- **源文件主权**：修权威源，然后重跑同一套验收关卡。
- **本地优先**：转写、分类、图注尽量跑在本机（faster-whisper + Ollama），全链路零云费用。
- **给人读的工作流**：最短的可用路径要看得见，实现细节排在它后面。

## 工具与语言

Python · Go · TypeScript · Vue · PowerShell · SQLite · PostgreSQL · LaTeX

## 关于本页

本页只列公开仓库；私有工作与私有验收产物有意不在此列出。
