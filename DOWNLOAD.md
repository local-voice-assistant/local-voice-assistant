# 下载与安装

**当前版本**：0.1.0（预发布）  
**系统要求**：Apple Silicon · macOS 14.2+

## 获取安装包

[前往 GitHub Releases](https://github.com/local-voice-assistant/local-voice-assistant/releases/latest)

每个版本提供两种安装包：

| 文件 | 说明 |
|------|------|
| `LocalVoiceAssistant-*-slim-arm64.dmg` | **精简版**：体积小；首次使用需在应用内下载默认识别模型（约 1.5GB） |
| `LocalVoiceAssistant-*-full-arm64.dmg` | **全量版**：已内置默认识别模型，安装后即可转写（安装包更大） |

请核对 Release 中的 `SHA256SUMS.txt`。版本元数据见 [`latest.json`](latest.json)（`url` 默认指向精简版；`variants.slim` / `variants.full` 为两份完整链接）。

## 首次打开被拦截？

当前使用临时签名；购买 Apple 开发者证书并公证后将减少拦截。

1. 右键 App →「打开」
2. 或「系统设置 → 隐私与安全性」→「仍要打开」
3. 必要时：

```bash
xattr -dr com.apple.quarantine "/Applications/本地语音助手.app"
```

返回 [首页](README.md)
