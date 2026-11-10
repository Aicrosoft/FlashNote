# 流光笔记 FlashNote - 让每一道流光，都有处安放。

> **你只管写，剩下的交给我。**
> 侧边栏 Markdown 专注创作，所见即所得，图表公式信手拈来；一键直发静态博客，长期内容自动沉淀为专栏、汇编成书。每一道流光，都替你安放成章。

[![Release](https://img.shields.io/github/v/release/Aicrosoft/FlashNote?color=blue&label=Latest%20Release)](https://github.com/Aicrosoft/FlashNote/releases)
[![Help Documentation](https://img.shields.io/badge/Docs-%E5%9C%A8%E7%BA%BF%E5%B8%AE%E5%8A%A9%E6%96%87%E6%A1%A3-brightgreen)](https://aicrosoft.com/apps/flashnote/help/)
[![License](https://img.shields.io/badge/License-Proprietary-orange)](https://aicrosoft.com/)

📖 **官方在线帮助文档**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)  
💬 **问题反馈与建议**: [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues)

**多语言完整文档 (Complete Multi-Language Editions)**:  
[🇨🇳 简体中文 (完整版)](README.zh-CN.md) | [🇺🇸 English (Full Edition)](README.en.md) | [🇭🇰 繁體中文 (完整版)](README.zh-TW.md) | [🇯🇵 日本語 (完全版)](README.ja.md)

---

> [!WARNING]
> ⚠️ **桌面版特别提示 (Experimental Preview)**：
> 流光笔记桌面端（macOS / Windows / Linux）目前为**实验性产品**，基于 Tauri 2.0 跨平台底层架构构建。如果您在使用过程中遇到任何问题、异常崩溃或有任何交互改进建议，非常欢迎随时在 [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues) 中提出反馈与问题，我们将持续迭代优化！

---

## 🚀 跨平台桌面端下载 (Downloads & Releases)

您可以在 [GitHub Releases](https://github.com/Aicrosoft/FlashNote/releases) 页面获取对应操作系统的最新安装包：

| 操作系统    | 安装包格式           | 说明                                                |
| :---------- | :------------------- | :-------------------------------------------------- |
| **macOS**   | `.dmg` / `.app.zip`  | 苹果电脑安装镜像 / 免安装应用归档                   |
| **Windows** | `.exe` / `.msi`      | 现代化 NSIS 安装向导 / 经典 Windows Installer       |
| **Linux**   | `.AppImage` / `.deb` | 免安装跨发行版单文件便携包 / Debian & Ubuntu 安装包 |

---

## 🌟 核心功能特性 (Feature Highlights)

### 1. ✍️ 极致纯粹的沉浸式 Markdown 创作

- **极速冷启动与开屏零卡顿**：重构底层资源加载调度与依赖按需懒加载，彻底根除打开后前 10 多秒按钮卡顿假死问题，实现首屏秒级即点即用；
- **所见即所得编辑器**：基于 Tiptap (ProseMirror) 现代内核，实时渲染 Markdown 语法，代码高亮、表格、列表、任务项开箱即用；
- **打字彻底消除延迟**：标题输入框与正文采用微观状态隔离，连续打字不再频繁触发全文档重渲染与磁盘写入，回车一键平滑跳入正文首行；
- **Markdown 标题拷入智能净化**：从外部网页复制标题时，自动剥离前导 `#`、行内反引号、加粗等排版噪声，光标智能定位末尾；
- **KaTeX 数学公式原生排版保真**：全层级自然块级流排版，支持矩阵 (Matrix)、分段函数 (Cases)、高阶积分上下标完美渲染，零遮挡零截断。

### 2. 🌐 深度网页剪藏与离线安全存储

- **论坛全楼层讨论完整捕获**：深度适配技术社区（如 Discourse / LINUX DO 等），点击剪藏按钮，自动将视口内加载的楼主主贴与所有参与讨论的楼层内容整齐捕获并导入笔记；
- **右键深度摘要，完整保留长文主贴**：右键“摘要网页内容”解除机械字数截断限制，完整提取主贴全部多级小节、代码块与高清配图，自动过滤无关评论杂音；
- **网络图片全自动离线到本地**：每次剪藏网页内容后，系统自动在后台执行远程资源一键离线，将文章引用的所有网络图片秒级下载并安全存入本地 OPFS，告别原帖删图、图床失效与防盗链拦截。

### 3. 🛡️ 防误删安全机制与 Notion 紧凑工作台

- **防误删人机工程**：同名清理弹窗将“仅将当前选中文档移入废纸篓”设为醒目默认选项，其他副本 100% 完好无损；“全部移入废纸篓”配有 5 秒可点击的「撤销恢复」通知，手误秒级还原；
- **Notion 属性内聚工作台**：顶部操作栏整合：目录与分类紧凑并列，修改路径与标签不再大幅横移鼠标；独立放置“转为书籍专栏”入口；
- **底部状态栏极简呼吸设计**：隐去重复标题，以轻量呼吸风格专注于实时字数统计、编辑保存状态与网络就绪情况，守护沉浸无扰的写作环境。

### 4. ☁️ 稳定多端云同步与 Git 静态博客直发

- **大文件 4MB 分块流式切片同步**：支持网盘大文件切片上传，接入 Precreate MD5 校验和序列与最终合成机制，彻底杜绝大附件超时失败；
- **状态机中断自愈与断点恢复**：网络抖动导致同步中断时，状态机自动安全回滚并支持断点自愈，确保本地沙箱与云端完全一致；
- **英文短名 (Slug) 智能消歧**：重名笔记自动追加序号平滑化解全路径冲突，普通日常随手记 100% 保护 AI 额度，零浪费 Token；
- **Git 远程博客一键直发**：支持将文章直连推送至 GitHub、Azure DevOps 等代码仓库，一键构建静态博客，精准标注发布生命周期。

### 5. 📚 专栏汇编出书与多格式高清导出

- **专栏汇编成书**：将日常积累的系列文章一键编排为章节目录；
- **标准 EPUB 3.0 / Markdown 打包**：内置专业封面设计与排版模板，一键导出可在各类电子阅读器中流畅阅读的标准电子书；
- **纯前端离线 PlantUML 转 Mermaid 引擎**：无需搭建 Java 服务器，纯前端秒级转译；支持双模平移缩放预览与无损 SVG / 2x 高清 PNG 导出。

### 6. 🤖 AI 智能辅助长篇创作

- **创作生成自动收起**：点击执行创作生成后，微调卡片立即自动收起，正文区域完整展现打字机式流式生成；
- **生成过程一键中止**：AI 正在生成时若再次展开面板，按钮自动反转为醒目的红色「■ 停止生成」，点击即刻停止；
- **超长篇幅与多文风基调**：支持 5000 字以上史诗长篇与 8000 字以上传奇长文分小节结构化推进；提供“默认自然、通俗生动、理工严谨、商务公文、优美文学、幽默风趣”等 6 种文风基调。

---

## 💬 帮助与技术支持 (Help & Feedback)

- 📖 **官方在线帮助文档**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)
- 🐞 **问题反馈与建议**: 欢迎在 [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues) 中提交 Bug 报告或体验建议。
