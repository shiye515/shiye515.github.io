---
layout: default
title: r2-temp
description: 临时文件服务：客户端上传到私有 R2，并拿到 24 小时有效的签名下载 URL
repository_url: https://github.com/shiye515/r2-temp
---

[back](../)

## Temporary File Service

一个面向 AI、桌面端与自动化工作流的临时文件服务：客户端无需持有云存储凭据即可上传，并获得一个有效期为 24 小时、直连 R2 的下载 URL。

### 亮点

- 客户端不保存云存储凭据
- 原始二进制流上传，避免 multipart 或 base64 缓冲
- 固定 24 小时、单对象绑定的 SigV4 GET URL
- 私有 R2 存储，支持 Range 下载
- 内置 MIME、大小校验、客户端 ID、限流和安全日志控制

### links

- [GitHub](https://github.com/shiye515/r2-temp)
- [API 文档](https://github.com/shiye515/r2-temp/blob/main/docs/api.md)
- [私有化部署指南](https://github.com/shiye515/r2-temp/blob/main/docs/self-hosting.zh.md)
- [feedback](https://github.com/shiye515/shiye515.github.io/issues)
- [privacy-policy](./privacy-policy.html)

### 隐私政策

见 [privacy-policy](./privacy-policy.html)
