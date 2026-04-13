# 01-ffmpeg/cmd
FFmpeg 命令行实战笔记，按场景分类整理，包含命令、参数说明、避坑指南。

## 📂 子目录说明
| 子目录 | 核心内容 |
|--------|----------|
| [basic/](sslocal://flow/file_open?url=.%2Fbasic%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | 基础命令：转码、格式转换、音视频提取 |
| [filter/](sslocal://flow/file_open?url=.%2Ffilter%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | 滤镜命令：裁剪、水印、缩放、倍速等 |
| [extract/](sslocal://flow/file_open?url=.%2Fextract%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | 原始数据提取：YUV/PCM 提取、播放、报错解决 |
| [live/](sslocal://flow/file_open?url=.%2Flive%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | 直播命令：推流、拉流、RTMP/HLS 处理 |

## ✅ 核心命令清单（持续更新）
### 1. 基础转码
```bash
# 无损转码，复制音视频流
ffmpeg -i input.mp4 -c copy output.mp4
# H.264 编码转码，控制画质
ffmpeg -i input.mp4 -c:v libx264 -crf 23 -c:a aac output.mp4
