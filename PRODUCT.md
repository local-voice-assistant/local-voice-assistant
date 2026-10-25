# 软件介绍

本地语音助手是面向 Mac 的**本地优先语音工作台**：转写与听写是底座，洞察与技能把会议变成可执行结果，工作区让你边听边互动；CB08 录音卡与 AI Passport 电子工牌可作随身输入。

<p align="center">
  <img src="assets/hero.jpg" alt="本地语音助手工作区与扩展硬件" width="860"/>
</p>

---

## 核心功能

### 实时转写

- 流式预览 + 离线定稿，说话过程中即可看到文字
- 说话人区分，便于回顾「谁说了什么」
- 支持热词与精修；音频默认只在本机处理

### 系统听写

- 按住修饰键开始听写，松开结束
- 字幕式 HUD，注入到当前应用光标处
- 可选用麦克风、系统音频，或已连接的录音卡 / 工牌作为音源

---

## 特色能力

<table>
  <tr>
    <td width="50%" align="center" valign="top">
      <img src="assets/crop-insight.jpg" alt="洞察卡片" width="400"/><br/>
      <sub>旁听洞察</sub>
    </td>
    <td width="50%" align="center" valign="top">
      <img src="assets/crop-docs.jpg" alt="产出文档" width="400"/><br/>
      <sub>技能产出与资料库</sub>
    </td>
  </tr>
</table>

### 洞察

旁听模式下本机生成洞察卡片（建议、待办、风险等）。默认**不自动执行**，由你确认后再行动。

### 技能

| 技能 | 作用 |
|------|------|
| 会议总结 | 生成结构化纪要 |
| 待办提取 | 整理待办列表 |
| 风险识别 | 识别讨论中的风险点 |
| 会议备忘 | 记入值得记住的要点 |
| 任务规划 | 拆成可执行步骤 |
| 网络搜索 | 检索外网事实并附出处 |

### 工作区实时互动

转写进行中即可提问、对卡片追问、把结果落到文档。

```mermaid
flowchart TB
  audio[声音输入] --> asr[本机转写]
  asr --> live[时间线与说话人]
  asr --> listen[旁听洞察]
  listen --> cards[洞察卡片]
  cards --> ask[工作区追问]
  ask --> skills[技能产出]
  skills --> docs[纪要待办文档]
```

---

## 扩展硬件

<p align="center">
  <img src="assets/hardware.jpg" alt="CB08 与 AI Passport" width="820"/>
</p>

通过蓝牙接入。同一时间建议只由一个程序连接设备。

### CB08 录音卡

- 实时语音上行到本机转写 / 听写
- 支持设备上录音文件的列表与下载

### AI Passport 电子工牌

<p align="center">
  <img src="assets/ai-passport-photo.png" alt="AI Passport 电子工牌实物" height="360"/>
</p>

- 实时语音上行（设备上无录音文件分区）
- 三键控制会议：开始 / 停止 / 暂停与继续
- 长按可触发听写（听写音源需设为工牌时）

---

## 其它

- 主题 AI Bot：旁听 / 指令 / 混合模式
- 可选配置你自己的云端大模型 API（文本才会出本机）
- 数据目录：`~/Library/Application Support/本地语音助手/`

返回 [首页](README.md) · [使用教程](GUIDE.md) · [下载](DOWNLOAD.md) · [捐赠](DONATE.md)
