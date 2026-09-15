---
layout: default
title: AudiobookMaker
description: 把 EPUB / 文本转换成本地有声书的 macOS 应用
repository_url: https://github.com/shiye515/AudiobookMaker
---

[back](../)

## 讯音有声书 / AudiobookMaker

这是一个面向 macOS 的本地有声书制作工具。导入 EPUB 或文本后，应用会按目录层级拆分章节，并使用 CosyVoice3 + MLX 在本机批量合成音频，最终输出带章节的 M4B，便于同步到 iPhone 的 Books 中直接收听。

### 亮点

- EPUB 导入：保留封面、作者、字数与章节层级信息
- 节级章节拆分：按目录最小节切分，并能修正 Calibre / NCX 目录错位问题
- 全程本地推理：正文与音频均在本机处理，不上传书籍内容
- 批量合成：支持全书入队、暂停/继续、断点续传
- 音色选择：内置参考样本 + 零样本克隆，可为不同书籍设定默认音色
- 导出格式：M4B、分章 M4A、WAV，可保留封面、章节与元数据
- 轻量文本转语音：不建书也能直接合成单段文字

### 技术栈

- SwiftUI
- Apple Silicon + macOS 15+
- CosyVoice3
- MLX 本地推理
- M4B / AAC / 章节标记导出

### 链接

- [GitHub](https://github.com/shiye515/AudiobookMaker)
- [FAQ](https://github.com/shiye515/AudiobookMaker/blob/main/docs/FAQ.md)
- [反馈](https://github.com/shiye515/shiye515.github.io/issues)

### 截图

![书架](https://raw.githubusercontent.com/shiye515/AudiobookMaker/main/docs/screenshots/library.png)

![章节队列](https://raw.githubusercontent.com/shiye515/AudiobookMaker/main/docs/screenshots/book-detail.png)

![导出 M4B](https://raw.githubusercontent.com/shiye515/AudiobookMaker/main/docs/screenshots/export-m4b.png)

### 系统要求

- Apple Silicon Mac（M1 及以后）
- macOS 15+
- 建议 16GB+ 内存；首次下载模型约 2GB+

### 快速开始

```bash
git clone https://github.com/shiye515/AudiobookMaker.git
cd AudiobookMaker
open abm.xcodeproj
```

1. 等待 Swift Package 解析完成
2. 使用 Xcode 运行
3. 在应用内初始化模型并下载权重
4. 导入 EPUB 或文本，选择一键生成全书，再导出 M4B

### 免责声明

软件按“原样”提供。请遵守当地法律与版权，仅处理你有权使用的文本与声音。
