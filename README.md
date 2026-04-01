# 🌌 ZTMY_OS: Zutomayo Inspired Web OS Theme for Typecho
新手做的一个真夜中风味的基于typecho的动态博客主题，参考了真夜中官网风格

[![Typecho](https://img.shields.io/badge/Typecho-1.2+-00ff41?style=flat-square&logo=php)](https://typecho.org/)
[![License](https://img.shields.io/badge/License-MIT-7000cc?style=flat-square)](LICENSE)
---

## ✨ 核心特性 (SYSTEM_FEATURES)

本主题完全重构了博客的交互逻辑，将网页抽象为桌面环境：

- **📟 沉浸式开机序列 (Boot Sequence)**: 模拟系统自检动画，带有极具氛围感的 `ZTMY_OS` 加载界面。
- **🖥️ 窗口化多任务管理**: 所有的文章、设置、游戏均在独立的可拖拽窗口中运行。
- **💻 极客终端 (TERMINAL.exe)**: 
    - 支持交互式命令：`ls` (列出文章), `date`, `whoami`, `clear`, `mines`。
    - 纯原生 JavaScript 实现的命令解析。
- **📼 随身听模块 (WALKMAN)**: 
    - 拟物化磁带 UI 设计，支持 CSS 旋转动画效果。
    - 内置 25 首预设歌单逻辑（需手动配置音频资源）。
- **💣 经典扫雷 (MINESWEEPER)**: 
    - 完美复刻 Windows 经典扫雷，包含插旗、计时、自动展开等完整算法。
- **📺 CRT 视觉滤镜**: 
    - 纯 CSS 实现的扫描线 (Scanlines) 与屏幕闪烁特效，还原 90 年代显示器质感。
- **💬 信号捕获评论区**: 
    - 将 Typecho 评论系统重写为 `SIGNAL_ROOM` 风格。

---

## 📸 预览 (PREVIEW)

> *此处建议上传一张你博客的截图，然后替换下方的链接*
![Screenshot](images/Ayanami.png)

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
- **操作**: 在主题目录下新建 `music/` 文件夹。
- **对应**: 确保文件名与 `index.php` 中 `playlist` 数组定义的参数一致。

### 2. 背景图片 (Background)
默认使用 `images/Ayanami.png`。
- 如需更换，请修改 `style.css` 中的 `body` 背景或替换 `images` 目录下的同名文件。

### 3. 字体资源
本主题调用了 Google Fonts 的 `VT323` 和 `DotGothic16` 字体以保证像素视觉效果。

---

## 📜 常用终端命令 (COMMANDS)

在博客内打开 **TERMINAL** 窗口，你可以尝试输入：

| 命令 | 说明 |
| :--- | :--- |
| `ls` | 实时列出当前博客的所有文章标题 |
| `mines` | 从命令行直接启动扫雷程序 |
| `whoami` | 显示当前访客身份 |
| `help` | 查看所有可用指令 |

---

- **技术栈**: PHP (Typecho), Vanilla JS, CSS3.
- **Icons**: Emoji & Font Awesome.

欢迎通过 Issues 提交 Bug 或建议。如果你喜欢这个设计，请给一个 **Star** ⭐！
