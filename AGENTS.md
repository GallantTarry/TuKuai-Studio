# TuKuai-Studio Repository Rules

## Language & Internationalization Standard

1. **Portal Shell (`zh-Hant` Traditional Chinese)**:
   - The Studio entrance and host shell (`intro.html`, `index.html`), Studio section UI copy in `sections.json`, and Studio guides (`教程.md`, `assets/更新日志.md`) use **Traditional Chinese (`<html lang="zh-Hant">`)** rather than Simplified Chinese.
   - Do not convert `href="https://土块.art"` or existing binary media filenames (such as `audio/言叶之庭.aac`) when editing markup.

2. **All Embedded Tool Pages & Shared UI Libraries (Pure English Only)**:
   - **Every web page intended to be embedded inside `index.html`'s `<iframe id="component-frame">` MUST be written strictly in pure English (`<html lang="en">`)** — including `TuKuaiUI/TuKuaiUI.html`, `TuKuaiEXE/TuKuaiEXE.html`, and any new tool pages added under `sections.json`.
   - Shared UI libraries (such as `assets/tukuai-ui.min.js`) and generated HTML/code snippets exposed to users must likewise use pure English labels, defaults, aria-labels, console errors, and comments.
   - Match the unified Studio eyebrow spec on every embedded page: `<div class="header-eyebrow"><DOMAIN> / <TOOL-NAME></div>` (`11px` monospace, `letter-spacing: 2.2px`, `font-weight: 600`, `text-transform: uppercase`, `margin-bottom: 12px`) using the domain's accent color (`Comp` = `var(--blue)`, `Core` = `var(--green)`, `IO` = `var(--yellow)`, `Net` = `var(--purple)`, `Sys` = `var(--red)`).

3. **Bilingual Documentation (`README.md` + `README.zh-TW.md`)**:
   - Keep `README.md` in **English** with `English | [繁體中文](README.zh-TW.md)` on line 1, synchronized with `README.zh-TW.md` (`[English](README.md) | 繁體中文`).
