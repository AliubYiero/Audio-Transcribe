# AudioTranscribe - 音频转写工具

一个简洁的 Web 应用，用于将音频文件转写为文本。基于 SiliconFlow API，支持多种音频格式。

## 功能特性

- 支持拖拽上传或点击选择音频文件
- 支持 MP3、WAV、M4A、FLAC 等常见音频格式
- 实时显示转写进度和状态
- 转写结果支持编辑和复制
- API 配置保存在本地浏览器，数据安全
- 响应式界面设计

## 使用方法

1. 直接在浏览器中打开 `Audio Transcribe.html` 文件
2. 首次使用需要先在「配置页面」设置 API 信息：
   - API 地址（默认为 SiliconFlow 接口）
   - 模型名称（如 TeleAI/TeleSpeechASR）
   - API Key
3. 返回「识别页面」，上传音频文件即可开始转写

## 默认配置

- API 地址: `https://api.siliconflow.cn/v1/audio/transcriptions`
- 默认模型: `TeleAI/TeleSpeechASR`

## 技术栈

- 纯 HTML/CSS/JavaScript，无需构建
- 使用 OpenAI 兼容的音频转写 API
- 配置存储使用 localStorage

## 文件结构

```
Audio Transcribe/
├── Audio Transcribe.html    # 主应用文件
├── logo.svg                 # 应用图标
└── README.md                # 说明文档
```

## 注意事项

- API Key 仅保存在本地浏览器，不会上传到任何服务器
- 转写结果按句子自动换行显示
- 支持 Ctrl/Cmd + Enter 快捷键复制文本
