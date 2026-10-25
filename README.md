# 🎨 TuKuaiStudio CDN (土块影音组件极速分发)

> 100% 原生 Web Components 架构，零外部依赖，内置音频播放器 + 视频播放器 + 5 套流光主题样式。

---

## 🚀 极速 CDN 引用（免下载 · 零 CSS 配置）

直接在任何 HTML 网页中复制引入下面这一行：

```html
<!-- 🌟 土块 UI 极速 CDN 单文件全量引入 (包含音频+视频+所有流光主题样式) -->
<script src="https://cdn.jsdelivr.net/gh/GallantTarry/tukuaistudio@main/tukuai-ui.min.js"></script>
```

> **生产环境推荐（锁定版本）：**
> ```html
> <script src="https://cdn.jsdelivr.net/gh/GallantTarry/tukuaistudio@1.0.0/tukuai-ui.min.js"></script>
> ```

---

## 🎵 1. 音频播放器调用示例

```html
<tukuai-audio
    url="https://example.com/music.mp3"
    name="歌曲名称"
    artist="歌手名"
    cover="https://example.com/cover.jpg"
    mode="sunset"
    loop>
</tukuai-audio>
```

* `mode` 可选值：`dark`（默认极客黑）、`light`（温柔粉紫）、`sunset`（落日金橘）、`ocean`（深海青蓝）、`cyberpunk`（赛博魅紫）

---

## 🎬 2. 视频播放器调用示例

```html
<tukuai-player
    url="https://example.com/video.mp4"
    title="视频标题"
    pic="https://example.com/poster.jpg"
    mode="cyberpunk">
</tukuai-player>
```

* 内置特性：毛玻璃呼吸光环、中央微光大播放钮、自动闲置隐藏控制条、📸一键高清截帧、双击全屏/单击暂停。

---

## 📄 开源许可
MIT License © GallantTarry (土块)
