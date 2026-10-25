Ran find tukuai-ui files locally
Ran list TuKuai-Studio directory
Analyzed README.md:L1-56
Ran list TuKuaiUI directory
Analyzed TuKuaiUI.html:L1-150

为你整理了一份专业、美观、可以直接复制粘贴到 GitHub [TuKuai-Studio](https://github.com/GallantTarry/TuKuai-Studio) 的完整 `README.md` 文档：

```markdown
<div align="center">

# 🎨 TuKuai-UI (土块影音工坊)

> **极简 · 优雅 · 零依赖** —— 基于原生 Web Components 架构的现代化音视频播放组件库。  
> 仅需引入一行 JS，即可在任何网页直接使用 `<tukuai-audio>` 和 `<tukuai-player>`，内置全部毛玻璃视觉与 5 套流光主题，无需引入任何额外 CSS 文件！

[![jsDelivr](https://data.jsdelivr.com/v1/package/gh/GallantTarry/TuKuai-Studio/badge)](https://www.jsdelivr.com/package/gh/GallantTarry/TuKuai-Studio)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Web Components](https://img.shields.io/badge/Architecture-Web%20Components-blue.svg)](https://developer.mozilla.org/zh-CN/docs/Web/API/Web_components)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-0-success.svg)](#)
[![Theme: 5 Preset Modes](https://img.shields.io/badge/Themes-5%20Presets-pink.svg)](#)

</div>

---

## ✨ 核心特性

- 🚀 **零依赖 · 极速上手**：基于标准原生 Web Components（Custom Elements），不依赖 Vue / React / jQuery，无论是在静态 HTML 还是现代前端框架中都能无缝使用。
- 📦 **单文件自闭环**：CSS 样式全量封装在 JS 内部，无需额外引入样式表，避免 CSS 类名污染或样式丢失。
- 🌈 **5 套预设流光主题**：内置极客黑（Dark）、浪漫粉紫（Light）、落日金橘（Sunset）、深海青蓝（Ocean）、赛博魅紫（Cyberpunk），随心切换。
- 🎬 **全功能视频播放器**：支持毛玻璃浮雕光效、居中微光大播放钮、自动闲置隐藏控制条、📸 **一键高清画质截帧**、单击暂停与双击全屏。
- 📱 **响应式自适应**：原生适配桌面大屏、iPad 平板与手机端触控体验。

---

## ⚡ 极速 CDN 引入

在任何 HTML 文件的 `<head>` 或 `<body>` 中引入下面这一行即可完成安装：

```html
<!-- 🌟 土块 UI 极速 CDN 全量引入 (包含音频+视频+所有流光主题) -->
<script src="https://cdn.jsdelivr.net/gh/GallantTarry/TuKuai-Studio@v1.0.0/tukuai-ui.min.js"></script>
```

> [!TIP]
> **生产环境建议**：锁定版本号（如 `@v1.0.0`），避免未来主分支变动影响线上页面；开发测试时也可以使用 `@main` 追踪最新提交。

---

## 🎵 1. 音频播放器 (`<tukuai-audio>`)

### 快速示例
```html
<tukuai-audio
    url="https://your-domain.com/music.mp3"
    name="歌曲名称"
    artist="歌手名"
    cover="https://your-domain.com/cover.jpg"
    mode="sunset"
    loop>
</tukuai-audio>
```

### 属性配置表

| 属性名 | 类型 | 默认值 | 说明 |
| :--- | :--- | :--- | :--- |
| `url` | `String` | **必填** | 音频资源直链（MP3 / M4A / WAV 等） |
| `name` | `String` | `'未知音频'` | 歌曲/音频标题 |
| `artist` | `String` | `'未知艺术家'` | 演唱者 / 播客作者 / 演讲人 |
| `cover` | `String` | 内置默认封面 | 唱片封面图片直链 |
| `mode` | `String` | `'dark'` | 流光主题配色（见下方主题列表） |
| `loop` | `Boolean` | `false` | 是否开启单曲循环 |
| `autoplay` | `Boolean` | `false` | 是否自动播放（受浏览器媒体策略限制） |

---

## 🎬 2. 视频播放器 (`<tukuai-player>`)

### 快速示例
```html
<tukuai-player
    url="https://your-domain.com/video.mp4"
    title="我的高清视频"
    pic="https://your-domain.com/poster.jpg"
    mode="cyberpunk">
</tukuai-player>
```

### 属性配置表

| 属性名 | 类型 | 默认值 | 说明 |
| :--- | :--- | :--- | :--- |
| `url` | `String` | **必填** | 视频文件直链（MP4 / WebM 等） |
| `title` | `String` | `''` | 顶部悬浮的视频标题 |
| `pic` | `String` | `''` | 视频加载前的预览海报/封面图（Poster） |
| `mode` | `String` | `'dark'` | 流光主题配色（见下方主题列表） |
| `autoplay` | `Boolean` | `false` | 是否静音自动播放 |
| `loop` | `Boolean` | `false` | 是否循环播放 |

### 视频特色交互
- **📸 一键高清截帧**：点击控制条上的相机图标，直接在本地通过 Canvas 渲染并高速下载当前帧的无损 PNG 截图。
- **⌨️ 快捷手势**：
  - 单击画面：播放 / 暂停
  - 双击画面：进入 / 退出全屏
  - 自动感应：鼠标静止 2.5 秒后控制栏平滑淡出，轻微移动即刻浮现。

---

## 🎨 3. 5 大流光主题一览

通过指定 `mode="..."` 即可即时切换：

| 主题属性值 (`mode`) | 中文名称 | 视觉风格与色调 |
| :--- | :--- | :--- |
| `dark` | **极客黑（默认）** | 深空黑底 + 经典科技荧光黄点缀，沉稳深邃 |
| `light` | **温柔粉紫** | 柔雾粉紫光晕，适合二次元、轻快与治愈系页面 |
| `sunset` | **落日金橘** | 暖调晚霞落日渐变，流光溢彩，氛围感极佳 |
| `ocean` | **深海青蓝** | 浅海青碧渐变湛蓝，清爽通透，极具未来感 |
| `cyberpunk` | **赛博魅紫** | 霓虹紫金对撞，电竞与流光毛玻璃质感拉满 |

---

## 💻 完整独立 HTML 页面模板

直接新建一个 `.html` 文件，粘贴以下代码，双击即可在浏览器中完美运行：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TuKuai-UI 演示</title>
    <!-- 引入 CDN -->
    <script src="https://cdn.jsdelivr.net/gh/GallantTarry/TuKuai-Studio@v1.0.0/tukuai-ui.min.js"></script>
    <style>
        body {
            background: #0f172a;
            color: #fff;
            font-family: sans-serif;
            padding: 40px 20px;
            max-width: 800px;
            margin: 0 auto;
        }
        .gap { margin-bottom: 30px; }
    </style>
</head>
<body>

    <h2>🎵 音频组件示例</h2>
    <div class="gap">
        <tukuai-audio
            url="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3"
            name="示例音频"
            artist="TuKuai Studio"
            mode="ocean">
        </tukuai-audio>
    </div>

    <h2>🎬 视频组件示例</h2>
    <div class="gap">
        <tukuai-player
            url="https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4"
            title="落日流光视频"
            mode="sunset">
        </tukuai-player>
    </div>

</body>
</html>
```

---

## ⚠️ 注意事项与避坑指南

1. **中文乱码问题**：在本地新建 HTML 文件时，`<head>` 标签内必须声明 `<meta charset="UTF-8">`，避免 Windows 本地浏览器以 GBK 默认编码解析导致中文乱码。
2. **跨域截帧问题**：视频截图功能使用浏览器的 Canvas API，若视频资源存放在第三方服务器上，该服务器必须开启 CORS 允许跨域（即响应头带有 `Access-Control-Allow-Origin: *`），否则浏览器会出于安全策略拦截截图。

---

## 📄 开源许可证

本项目基于 [MIT License](LICENSE) 开源协议，欢迎自由使用、集成与二开！  
Author: [GallantTarry (土块)](https://github.com/GallantTarry)
```
