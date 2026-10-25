# 开源组件与模型声明

本地语音助手发行包可能包含或在运行时下载下列组件（非完整列表，以实际依赖为准）：

## 运行时 / 库

| 组件 | 许可（典型） | 说明 |
|------|--------------|------|
| Node.js | MIT 等 | 运行时 |
| sherpa-onnx / sherpa-onnx-node | Apache-2.0 | 本机 ASR / VAD / 声纹 / 标点 |
| @earendil-works/pi-coding-agent | 按其仓库许可 | Agent 运行时 |
| Fastify 及相关插件 | MIT | 本机 HTTP/WS |
| Silero VAD | 按其模型许可 | 语音活动检测 |

请自行查阅各上游仓库的 LICENSE 文件以获取完整条款。

## 识别模型（按需下载，默认不打进安装包）

| 模型 | 用途 |
|------|------|
| Zipformer bilingual | 流式预览 |
| Paraformer zh | 离线定稿 |
| SenseVoice | 多语种备选 |
| CAM++ | 说话人嵌入 |
| ct-transformer 标点 | 中英标点 |

模型权重由上游发布，再分发与商用条款以模型作者声明为准。本产品默认由用户在线下载，而非内置商用再分发。

## 录音压缩

停录后的录音由 macOS 自带的 `afconvert`（系统 AudioToolbox）编码为 AAC（`.m4a`）。本软件**不附带、不下载**任何第三方音频编码器或转码程序；非 macOS 环境不做压缩，录音保留为 WAV。
