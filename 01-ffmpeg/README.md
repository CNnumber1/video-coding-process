# 01-ffmpeg
FFmpeg 命令行、C 语言 API 开发相关学习内容，是音视频技术栈的核心基础。

## 🎯 模块目标
- 熟练掌握 FFmpeg 常用命令，解决实际音视频处理需求
- 理解 FFmpeg 架构与核心数据结构，掌握 C 语言 API 开发
- 积累命令行报错解决方案，形成可复用的实战笔记

## 📂 子目录说明
| 子目录 | 核心内容 | 学习进度 |
|--------|----------|----------|
| [cmd/](sslocal://flow/file_open?url=.%2Fcmd%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | FFmpeg 命令行实战（转码、裁剪、水印、推流/拉流等） | 70% |
| [dev/](sslocal://flow/file_open?url=.%2Fdev%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | FFmpeg C 语言 API 开发（音视频提取、格式转换等） | 10% |
| [docs/](sslocal://flow/file_open?url=.%2Fdocs%2F&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=) | FFmpeg 学习笔记、课程对应知识点、原理总结 | 30% |

## ✅ 已掌握核心命令
- 基础转码：`ffmpeg -i input.mp4 -c:v libx264 output.mp4`
- 原始数据提取：YUV/PCM 提取命令+报错解决方案
- 视频滤镜：裁剪(`crop`)、水印(`overlay/drawtext`)、缩放等
- 直播推拉流：RTMP/HLS 推流/拉流命令，本地测试方案
- 音视频合并/分割：concat 协议使用，input.txt 编写

## 📚 待学习内容
- FFmpeg C 语言 API 开发（解封装、解码、编码、封装全流程）
- 复杂滤镜链开发，自定义滤镜
- 硬件加速（NVENC/VAAPI）转码优化
- FFmpeg 源码编译与二次开发
