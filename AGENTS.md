# TuKuai-Studio Repository Rules

## Language & Internationalization Standard

1. **Portal Shell (`zh-CN` Simplified Chinese)**:
   - The Studio entrance and host shell (`intro.html`, `index.html`), Studio section Chinese UI copy in `sections.json`, and Studio guides (`教程.md`, `assets/更新日志.md`) use **Simplified Chinese (`<html lang="zh-CN">`)**, while keeping all existing English text intact.
   - **Exception (Preserved Traditional Chinese Verses)**: On `index.html`, keep the two classical poetic lines in Traditional Chinese verbatim:
     - `“彩縷織錦，方寸棲靈。<br>以智慧之度量，雕琢器皿之榮美。”`
     - `微塵出造化，氣息動生靈.`
   - Do not convert `href="https://土块.art"` or existing binary media filenames (such as `audio/言叶之庭.aac`) when editing markup.

2. **All Embedded Tool Pages & Shared UI Libraries (Pure English Only)**:
   - **Every web page intended to be embedded inside `index.html`'s `<iframe id="component-frame">` MUST be written strictly in pure English (`<html lang="en">`)** — including `TuKuaiUI/TuKuaiUI.html`, `TuKuaiEXE/TuKuaiEXE.html`, and any new tool pages added under `sections.json`.
   - Shared UI libraries (such as `assets/tukuai-ui.min.js`) and generated HTML/code snippets exposed to users must likewise use pure English labels, defaults, aria-labels, console errors, and comments.
   - Match the unified Studio eyebrow spec on every embedded page: `<div class="header-eyebrow"><DOMAIN> / <TOOL-NAME></div>` (`11px` monospace, `letter-spacing: 2.2px`, `font-weight: 600`, `text-transform: uppercase`, `margin-bottom: 12px`) using the domain's accent color (`Comp` = `var(--blue)`, `Core` = `var(--green)`, `IO` = `var(--yellow)`, `Net` = `var(--purple)`, `Sys` = `var(--red)`).

3. **Bilingual Documentation (`README.md` + `README.zh-CN.md`)**:
   - Keep `README.md` in **English** with `English | [简体中文](README.zh-CN.md)` on line 1, synchronized with `README.zh-CN.md` (`[English](README.md) | 简体中文`).
   - Do **not** describe or list individual components in the root README; keep it focused solely on TuKuai Studio's founding mission to provide convenience for programmers and the open-source world, and clearly state the licensing boundary: the main website design is **All Rights Reserved** (see root `LICENSE`), while each component is governed by the `LICENSE` file in its own component directory.
