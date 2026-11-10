# FlashNote - Every stream of inspiration finds its rightful place.

> **You just write, leave the rest to me.**
> Sidebar Markdown creation with WYSIWYG editing, effortless charts & math formulas; 1-click publishing to static blogs, transforming long-term thoughts into curated columns and compiled books. Every stream of inspiration finds its rightful place.

[![Release](https://img.shields.io/github/v/release/Aicrosoft/FlashNote?color=blue&label=Latest%20Release)](https://github.com/Aicrosoft/FlashNote/releases)
[![Help Documentation](https://img.shields.io/badge/Docs-Help%20Documentation-brightgreen)](https://aicrosoft.com/apps/flashnote/help/)
[![License](https://img.shields.io/badge/License-Proprietary-orange)](https://aicrosoft.com/)

📖 **Online Documentation**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)  
💬 **Issues & Feedback**: [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues)

**Languages**:  
[🇨🇳 简体中文](README.zh-CN.md) | [🇺🇸 English](README.en.md) | [🇭🇰 繁體中文](README.zh-TW.md) | [🇯🇵 日本語](README.ja.md)

---

> [!WARNING]
> ⚠️ **Desktop Experimental Preview Notice**:  
> FlashNote Desktop (macOS / Windows / Linux) is currently an **experimental preview** built on the cross-platform Tauri 2.0 framework. If you encounter any bugs, crashes, or usability issues, feedback is warmly welcome via [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues)!

---

## 🚀 Desktop Downloads & Releases

You can download the latest installers for your operating system from the [GitHub Releases](https://github.com/Aicrosoft/FlashNote/releases) page:

| Operating System | Package Format       | Description                                              |
| :--------------- | :------------------- | :------------------------------------------------------- |
| **macOS**        | `.dmg` / `.app.zip`  | Apple Disk Image / Standalone App Archive                |
| **Windows**      | `.exe` / `.msi`      | Modern NSIS Setup Wizard / Classic Windows Installer     |
| **Linux**        | `.AppImage` / `.deb` | Cross-Distro Portable AppImage / Debian & Ubuntu Package |

---

## 🌟 Feature Highlights

### 1. ✍️ Pure Immersive Markdown Authoring

- **Lightning-Fast Launch & Zero Freeze**: Overhauled startup resource scheduling and lazy loading, completely resolving the 10+ second initial freeze and delivering instant interactive readiness;
- **True WYSIWYG Editor**: Real-time rendering powered by Tiptap/ProseMirror with syntax highlighting, tables, task lists, and blockquotes out-of-the-box;
- **Zero-Latency Typing**: The title input is isolated into an internal micro-state, preventing full-document re-renders and unnecessary disk writes during typing; press Enter to smoothly focus on the first line of the body;
- **Clean Title Paste Sanitization**: Automatically strips leading `#`, backticks, and bold formatting when pasting titles from external sources;
- **Native KaTeX Math Formula Fidelity**: Full natural block-flow typesetting for matrices, piece-wise cases, and multi-tier calculus integrals with zero truncation.

### 2. 🌐 Next-Gen Web Clipper & Offline Media Archiving

- **Full Forum Discussion Capture**: Deeply tailored for technical forums (e.g. Discourse / LINUX DO). 1-click capture gathers the original post and all visible reply levels (`### #1 Author`, `### #2 Reply`...) into clean, structured notes;
- **Right-Click Deep Summary Without Character Limits**: Right-click "Summarize Web Content" mode removes mechanical length truncations, extracting full sections, code blocks, and high-res images while filtering out noise;
- **Automatic Offline Image Archiving**: Every clipping action automatically triggers a background offline sync, downloading all remote images into local sandboxed storage (OPFS) to safeguard against broken image hosts and hotlinking protection.

### 3. 🛡️ Safety UX & Notion-Style Metadata Header

- **Safer Note Cleanup**: In duplicate note cleanup dialogs, "Move only currently selected note to trash" is highlighted in prominent red as the default choice; "Move all to trash" includes a 5-second clickable Undo Toast for effortless recovery;
- **Compact Side-by-Side Metadata**: Folder and category pickers sit compactly side-by-side; the last column features a dedicated "Convert to Book" trigger with an intuitive open-book icon;
- **Distraction-Free Breathing Status Bar**: Omits redundant titles to deliver a calm breathing indicator focused purely on real-time word count, auto-save status, and network readiness.

### 4. ☁️ Resilient Multi-Platform Cloud Sync & 1-Click Blog Publishing

- **4MB Streaming Slices Eliminate Upload Timeouts**: Long e-books, extensive notes, and bulky attachments are automatically sliced into 4MB boundaries with pre-upload MD5 validation (`precreate`) and final server-side assembly (`create`);
- **State-Machine Recovery**: Network interruptions trigger safe rollbacks and breakpoint-resumed self-healing, ensuring absolute consistency between local storage and cloud drives;
- **Smart English Slug Disambiguation**: Duplicate titles smoothly append numbered suffixes (e.g. `ebookunpack-2`) to avoid route collisions; daily quick notes 100% exempt from AI calls to conserve quota;
- **Direct Git Static Blog Publishing**: Push articles directly to GitHub or Azure DevOps repositories with 1 click to trigger static site generators, with complete publish lifecycle tracking.

### 5. 📚 Long Columns & EPUB 3.0 E-Book Compilation

- **Column Compilation into Books**: Organize accumulated notes and series into structured book chapters;
- **Standard EPUB 3.0 & Markdown Bundles**: Built-in professional cover art and typography presets to generate e-books ready for Kindle, Apple Books, and e-readers;
- **Pure Client-Side PlantUML-to-Mermaid Transpilation**: Zero Java PlantUML backend needed; toggle between Code and Preview modes with pan-zoom and lossless SVG / 2x PNG exports.

### 6. 🤖 AI-Powered Long-Form Authoring

- **Auto-Collapsing Refiner Panel**: Clicking "Generate" instantly collapses the panel so you can watch streaming typewriter text unhindered;
- **1-Click Stop Generation**: Re-expanding the panel during generation turns the action button into a bold red "■ Stop Generation";
- **Epic & Legendary Length Support**: Structured multi-section generation for 5,000+ words (Epic) and 8,000+ words (Legendary); supports 6 writing tones (Natural, Engaging, Technical, Business, Literary, Humorous).

---

## 💬 Help & Feedback

- 📖 **Online Help Documentation**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)
- 🐞 **Issues & Suggestions**: Feel free to submit bug reports and feature requests via [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues).
