<div align="center">

# 🪁 TuKuai Studio (土块工坊)

> **给灵感，一点颜色。**  
> 面向开发者与编程爱好者的现代化实用组件与工程积木工坊。

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)
[![Architecture: Modular](https://img.shields.io/badge/Architecture-Modular%20Blocks-blue.svg?style=flat-square)](#)
[![Zero Dependencies](https://img.shields.io/badge/Philosophy-Zero%20Dependencies-brightgreen.svg?style=flat-square)](#)
[![Spectrum: 5 Domains](https://img.shields.io/badge/Spectrum-5%20Domains-orange.svg?style=flat-square)](#)
[![Online Demo](https://img.shields.io/badge/Online-Studio%20Home-6366f1.svg?style=flat-square)](https://xn--2esp7m.xn--udsye.art/)

<p align="center">
  <a href="#-工坊愿景">工坊愿景</a> •
  <a href="#-五大领域规划">五大领域规划</a> •
  <a href="#-已上线组件-comp--tukuai-ui">已上线组件</a> •
  <a href="#-设计理念">设计理念</a> •
  <a href="#-在线体验">在线体验</a> •
  <a href="#-参与共建">参与共建</a>
</p>

</div>

---

## 🌟 工坊愿景

**TuKuai Studio（土块工坊）** 不是某一个单一的前端播放器或孤立工具，而是一座**为其他程序员与编程爱好者精心打造的“工程积木工坊”**。

在软件开发过程中，我们经常遇到类似困境：为了实现一个基础高频的能力，不得不引入臃肿庞大的第三方依赖，或者为了调整一段界面动效而陷入复杂的配置泥潭。

土块工坊的初衷就是**化繁为简**：
- 沉淀各个领域实用、优雅、小而美的能力；
- 提炼为**即插即用、零外部依赖、自闭环**的高质量工程积木；
- 为探索编程、渴望快速构建产品的开发者与爱好者，提供开箱即用的技术便捷。

---

## 🗺️ 五大领域规划

工坊以「五色光谱」为基调，聚焦现代软件工程的五个关键维度进行长期沉淀与组件孵化：

<table>
  <thead>
    <tr>
      <th width="90">领域标识</th>
      <th width="110">中文定位</th>
      <th width="70" align="center">色调</th>
      <th>名人箴言 / 核心理念</th>
      <th>规划覆盖方向</th>
      <th width="100" align="center">当前状态</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong><code>Comp</code></strong></td>
      <td><strong>组件与界面</strong></td>
      <td align="center">🔵 蓝色</td>
      <td><em>"Simple things should be simple, complex things should be possible."</em><br>— Alan Kay</td>
      <td>原生 Web Components、影音播放器、桌面轻量 GUI 控件（TuKuai-UI、JUI 等）</td>
      <td align="center"><span style="color: #10b981;">● 已首发上线</span></td>
    </tr>
    <tr>
      <td><strong><code>Core</code></strong></td>
      <td><strong>核心与算法</strong></td>
      <td align="center">🟢 绿色</td>
      <td><em>"We can only see a short distance ahead, but we can see plenty there that needs to be done."</em><br>— Alan M. Turing</td>
      <td>核心计算算法、几何调色引擎、轻量动画物理演算、通用数据结构基础库</td>
      <td align="center"><span>◌ 规划建设中</span></td>
    </tr>
    <tr>
      <td><strong><code>IO</code></strong></td>
      <td><strong>数据与流转</strong></td>
      <td align="center">🟡 黄色</td>
      <td><em>"The fundamental problem of communication is that of reproducing at one point either exactly or approximately..."</em><br>— Claude E. Shannon</td>
      <td>文本/文件极速读写解析、二进制数据流转换、文档格式轻量处理、本地配置持久化</td>
      <td align="center"><span>◌ 规划建设中</span></td>
    </tr>
    <tr>
      <td><strong><code>Net</code></strong></td>
      <td><strong>网络与协议</strong></td>
      <td align="center">🟣 紫色</td>
      <td><em>"The Web as I envisaged it, we have not seen it yet. The future is still so much bigger than the past."</em><br>— Sir Tim Berners-Lee</td>
      <td>轻量 HTTP/WebSocket 通信封装、极简 RPC 客户端、本地临时隧道与 P2P 互联工具</td>
      <td align="center"><span>◌ 规划建设中</span></td>
    </tr>
    <tr>
      <td><strong><code>Sys</code></strong></td>
      <td><strong>系统与底座</strong></td>
      <td align="center">🔴 红色</td>
      <td><em>"UNIX is basically a simple operating system, but you have to be a genius to understand the simplicity."</em><br>— Dennis M. Ritchie</td>
      <td>系统环境探针、高精度硬件定时器、跨平台系统互操作桥接、开发提效自动化脚本</td>
      <td align="center"><span>◌ 规划建设中</span></td>
    </tr>
  </tbody>
</table>

---

## 🚀 已上线组件：Comp / TuKuai-UI

工坊首个落地的实用组件为 **TuKuai-UI（现代化音视频 Web Components 组件库）**：

> **极简 · 优雅 · 零依赖** —— 仅需引入一行 JS，即可在任何网页直接使用 `<tukuai-audio>` 与 `<tukuai-player>`，无需额外打包或引入 CSS！

### 核心亮点
- ⚡ **一行引入，即插即用**：基于原生 Web Components（Custom Elements），无需安装庞大框架，纯 HTML 或 Vue/React 项目皆可直接渲染。
- 🎨 **内嵌样式与毛玻璃光效**：所有 CSS 全部封装在组件内部 Shadow DOM，杜绝全局类名污染与样式打架。
- 🌈 **5 套预设流光主题**：极客黑（Dark）、温柔粉紫（Light）、落日金橘（Sunset）、深海青蓝（Ocean）、赛博魅紫（Cyberpunk）。
- 🎬 **细腻的交互细节**：居中微光悬浮播放键、键盘全快捷键支持、双击全屏、以及📸 **一键无损高清画质截帧**。

### 极速接入代码

```html
<!-- 1. 引入土块 UI 脚本 (一行 CDN，包含音频+视频+所有流光主题) -->
<script src="https://cdn.jsdelivr.net/gh/GallantTarry/TuKuai-Studio@v1.0.0/tukuai-ui.min.js"></script>

<!-- 2. 在页面中直接调用标签 -->
<tukuai-player src="media/demo.mp4" theme="sunset"></tukuai-player>
<tukuai-audio src="media/demo.mp3" theme="ocean"></tukuai-audio>
```

---

## 💎 设计理念

1. **Zero Dependencies（零依赖偏执）**  
   拒绝动辄数百 MB 的臃肿依赖树。尽可能充分发挥现代原生语言与运行时的核心能力，保持极致的纯净与轻巧。
2. **Self-Contained（单文件自闭环）**  
   不管是前端组件还是后端工具类，力求单文件或模块自包含全部必要逻辑，降低接入成本。
3. **Aesthetic First（质感与交互并存）**  
   工具不应只是冷冰冰的代码。五色流光、毛玻璃质感与舒适的阻尼微动效，让每一次开发过程都具有愉悦感。
4. **Developer-Friendly（对开发者真正友好）**  
   设计符合直觉的 API，提供开箱即用的范例和详尽文档，方便不同阶段的编程爱好者学习与借鉴。

---

## 🌐 在线体验

欢迎访问土块工坊在线主页，亲自感受五色光谱导航与组件实效：

- 🔗 **工坊官网**：[https://xn--2esp7m.xn--udsye.art/](https://xn--2esp7m.xn--udsye.art/)
- 📖 **配置与扩展指南**：[如何用 sections.json 拓展工坊工具板块 (教程.md)](教程.md)

---

## 🤝 参与共建

土块工坊是一个持续扩展、充满生命力的极客实验室。如果你也对打造“小而美”的高质量工程组件充满热情，非常欢迎：
- 提出你希望工坊孵化的组件想法（[Issues](https://github.com/GallantTarry/TuKuai-Studio/issues)）
- 提交 PR，将你编写的 `comp`、`core`、`io`、`net`、`sys` 工具积木接入工坊
- 共同交流，让编程更有趣、更轻盈！

---

## 📄 开源许可证

本项目基于 [MIT License](LICENSE) 开源发布。自由使用，尽情创造。
