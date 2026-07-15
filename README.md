<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/mogu-ai-icon.png" width="112" alt="MOGU AI" />
</p>

<h1 align="center">MOGU AI 1.5.3</h1>

<p align="center">
  <strong>Agent 模型 · 本机 Agent · ComfyUI 创作 · 视频合成</strong><br>
  <sub>面向 Windows 的本地 AI 创作桌面应用。模型和作品留在自己的电脑。</sub>
</p>

<p align="center">
  <a href="https://github.com/ly136148277-netizen/mogu-ai-releases/releases/download/v1.5.3/MOGU-AI-Setup-1.5.3.exe"><strong>下载安装版</strong></a>
  ·
  <a href="https://github.com/ly136148277-netizen/MoguAI">查看源码</a>
  ·
  <a href="https://github.com/ly136148277-netizen/MoguAI/issues">反馈问题</a>
</p>

---

## MOGU AI 是什么

MOGU AI 把本地模型、电脑 Agent、ComfyUI 工作流和视频拼接放进一个桌面窗口。你可以下载 Agent 模型、让 Agent 操作本机、导入自己的 ComfyUI 工作流生成图片或视频，再把多个短镜头按时间线拼成长片。

它不是云端生成网站。Ollama、PAI、ComfyUI 和 FFmpeg 都运行在本机；是否使用联网模型由你自己决定。

<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/01-home-v153.png" width="900" alt="MOGU AI 1.5.3 首页" />
</p>

---

## 当前版本包含什么

### Agent 模型

- 浏览并下载 GGUF 模型
- 下载完成后导入 Ollama，在本机离线使用
- 管理已下载模型和下载任务
- Agent 引导模型支持三种方式：内置教程、本机 Ollama、联网 API
- 联网 API 支持 DeepSeek、OpenAI、通义千问、Kimi 和自定义 OpenAI 兼容地址

<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/02-agent-models-v153.png" width="900" alt="Agent 模型页面" />
</p>

### 本机 Agent

- 用自然语言打开 ComfyUI、列出工作流、搜索文件和备份项目
- 可以询问 MOGU AI、环境安装和创作台的使用方法
- 支持 PAI 的分级权限与危险操作确认
- 支持定时关机，长时间出片后可自动关闭电脑
- 办事走本机 PAI；引导和答疑可选内置、本地或联网模型

<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/03-agent-v153.png" width="900" alt="MOGU AI Agent 页面" />
</p>

### ComfyUI 创作台

- 导入自己的文生图和图生视频工作流
- 分开填写人物描述与动作描述
- 选择分辨率、清晰度和视频时长
- 尽量把提示词及参数写入兼容的 ComfyUI API 工作流
- 文生图成品可继续传给图生视频阶段
- 显示生成进度和输出预览
- 可中断当前 ComfyUI 任务并清空队列

工作流需要与任务和模型适配。优先使用 ComfyUI 的 **Save (API Format)**；特殊节点或特殊连线可能无法自动覆盖参数。

<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/04-studio-v153.png" width="900" alt="ComfyUI 创作台" />
</p>

### 视频合成

- 把多个短视频按时间线顺序排列
- 使用 FFmpeg 一键首尾拼接成长视频
- 首次使用时自动准备 FFmpeg
- 合成后可直接预览结果
- 可打开 Shotcut、剪映或自定义工具继续裁剪、转场和加字幕

<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/05-compose-v153.png" width="900" alt="视频合成时间线" />
</p>

### 一键环境

- 检查和启动 Ollama
- 安装、选择并连接 PAI
- 扫描本机 ComfyUI
- 安装便携 FFmpeg，无需手动配置 PATH
- 首页与创作台直接显示四项环境状态

<p align="center">
  <img src="https://raw.githubusercontent.com/ly136148277-netizen/mogu-ai-releases/main/docs/images/v1.5.3/06-setup-v153.png" width="900" alt="MOGU AI 一键环境页面" />
</p>

---

## 1.5.3 本次更新

- 重新整理首页和侧栏：Agent模型、Agent、ComfyUI创作、视频合成、环境
- 新增可视化 ComfyUI 创作台，可选择工作流并填写人物、动作和生成参数
- 新增视频时间线与一键拼接，可接入外部剪辑工具细修
- 新增环境中心，统一检查 Ollama、PAI、ComfyUI 和 FFmpeg
- 改进任务进度、取消任务和生成结果预览
- 安装程序支持选择安装位置并在开始前确认
- 安装完成后自动创建桌面快捷方式
- Windows 程序与快捷方式改为圆形蘑菇图标

---

## 安装与使用

### 推荐：安装版

1. 下载 **MOGU-AI-Setup-1.5.3.exe**
2. 双击运行，选择安装位置
3. 点击安装，完成后从桌面的圆形蘑菇图标启动
4. 首次打开进入「环境」，按需要配置 Ollama、PAI、ComfyUI 和 FFmpeg

### 便携版

下载 **MOGU.AI.1.5.3.exe** 后直接运行，不写入安装目录。长期使用仍建议安装版。

### 最低环境

- Windows 10 / 11，64 位
- MOGU AI 本体约 300 MB 可用空间
- 本地 Agent 模型需要额外模型空间，通常为数 GB
- 聊天和本地模型：需要 Ollama
- ComfyUI 创作：需要 PAI 与 ComfyUI
- 视频拼接：需要 FFmpeg，可在软件内安装

---

## 下载文件

**安装版（推荐）**

- 文件：`MOGU-AI-Setup-1.5.3.exe`
- 大小：83.3 MB
- SHA-256：`B9AB962C844335B2EE61622E394D9195C6F27194C2857E05C32FA8C453A682F0`

**便携版**

- 文件：`MOGU.AI.1.5.3.exe`
- 大小：82.8 MB
- SHA-256：`E0D1491ADEE348E84205FF903AE4D6BC257EFDD019EEF6F51571966C6A790E1E`

`latest.yml` 和 `.blockmap` 供应用内自动更新使用，普通用户不需要单独下载。

---

## 开源与反馈

- 源码与完整文档：https://github.com/ly136148277-netizen/MoguAI
- 问题反馈：https://github.com/ly136148277-netizen/MoguAI/issues
- 许可证：MIT
- 历史版本：[MOGU AI 1.4.0](https://github.com/ly136148277-netizen/mogu-ai-releases/releases/tag/v1.4.0)

