# 🌌 ZTMY_OS: Zutomayo Inspired Web OS Theme for Typecho

[![Typecho](https://img.shields.io/badge/Typecho-1.2+-00ff41?style=flat-square&logo=php)](https://typecho.org/)
[![License](https://img.shields.io/badge/License-MIT-7000cc?style=flat-square)](LICENSE)

> **ZTMY_OS V14.1**: （Zutomayo）风格的 Typecho 动态博客主题。它不只是一个皮肤，而是一个运行在浏览器里的复古 Web 操作系统与在线空间。

---

## ✨ 核心特性 (SYSTEM_FEATURES)

本主题完全重构了博客的交互逻辑，将网页抽象为桌面环境：

- **📟 沉浸式开机序列 (Boot Sequence)**: 
    - 模拟系统自检动画，带有极具氛围感的 `ZTMY_OS` 加载界面。
    - 启动完成后会自动弹出 **系统欢迎指令框 (Welcome Message)** 和 **节日彩蛋贴片 (XMAS_PATCH)**。
- **🖥️ 窗口化多任务管理**: 
    - 所有的文章 (`LOGS`)、设置、游戏均在独立的可拖拽窗口中运行。
    - 文章列表化身文件管理器，支持按分类检索和全局搜索。
- **💻 极客终端 (TERMINAL.exe)**: 
    - 支持交互式命令：`ls` (列出文章), `date`, `whoami`, `clear`, `mines`。
    - 纯原生 JavaScript 实现的命令解析，带有专属的 `root@kyokuya:~$` 提示符。
- **📡 匿名聊天大厅 (SIGNAL_ROOM)**: 
    - 桌面直接内嵌了基于 Hack.chat 的无缝聊天室 (`?zutomayo_lobby`)，访客可以直接进行实时交流。
- **📼 随身听模块 (WALKMAN)**: 
    - 拟物化磁带 UI 设计，支持 CSS 磁带转轮旋转动画。
    - 内置 25 首预设歌单逻辑（需手动配置音频资源）。
- **💣 经典扫雷 (MINESWEEPER)**: 
    - 完美复刻 Windows 经典扫雷，包含插旗、计时、自动展开等完整算法。
- **📺 视觉滤镜 & 信号评论区**: 
    - 纯 CSS 实现的 CRT 扫描线 (Scanlines) 与屏幕闪烁特效。
    - 将 Typecho 原生评论系统重写为赛博朋克风格的“截获信号”区。

---

## 📦 安装指南 (INSTALLATION)

1. **克隆/下载仓库**: 
   点击 `Code` -> `Download ZIP` 并解压。
2. **上传至服务器**: 
   将文件夹上传到 Typecho 安装目录下的 `/usr/themes/`。
3. **启用主题**: 
   登录 Typecho 后台 -> `控制台` -> `外观` -> `启用 ZTMY_OS`。

---

## 🛠️ 关键配置说明 (CONFIGURATION)

### 1. 音乐文件 (Music Setup)
由于版权和体积限制，本仓库不包含 `.mp3` 文件。
- **操作**: 在主题目录下手动新建 `music/` 文件夹。
- **对应**: 确保你的 `.mp3` 文件名与 `index.php` 中 `playlist` 数组定义的 `file` 参数完全一致（如 `milabo.mp3`）。

### 2. 背景图片 (Background)
默认调用 `images/Ayanami.png`。
- 如需更换，请将新图片上传至 `images` 文件夹，并修改 `index.php` 头部或替换同名文件。

### 3. 字体资源
本主题调用了 Google Fonts 的 `VT323` (代码终端) 和 `DotGothic16` (像素日文) 字体以保证视觉质感。

---

## 📜 常用终端命令 (COMMANDS)

在桌面打开 **TERMINAL** 窗口，尝试输入以下指令：

| 命令 | 说明 |
| :--- | :--- |
| `ls` | 实时打印当前博客的所有文章标题 |
| `mines` | 从命令行直接触发并启动扫雷程序 |
| `date` / `whoami` | 获取当前系统时间 / 访客身份 |
| `clear` | 清屏 |

---

## 🤝 贡献与感谢

- **技术栈**: PHP (Typecho), Vanilla JS, CSS3.
- **外部接入**: Hack.chat (Chatroom)

欢迎通过 Issues 提交 Bug 或建议。如果你喜欢这个设计，请给一个 **Star** ⭐！
