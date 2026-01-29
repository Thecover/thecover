# THE COVER

### 🛡️ A Retro-Style Disk Usage Analyzer for Linux

> Design by thecover
> 


## 📖 简介 (Introduction)

**THE COVER** 是一款基于 Go 语言开发的高性能 Linux 磁盘空间分析工具。与传统的 `du` 或 `ncdu` 不同，THE COVER 将现代化的**并发扫描技术**与怀旧的 **8-bit 像素美学**完美融合。

它专为那些厌倦了枯燥命令行的极客设计——在通过 TUI (终端图形界面) 高效管理磁盘空间的同时，也能享受到独特的视觉体验。

## ✨ 核心特性 (Features)

- **🚀 极速并发扫描 (Blazing Fast)**
利用 Go 语言强大的 `Goroutine` 并发模型，多线程异步计算文件夹大小，秒级响应，告别 I/O 阻塞卡顿。
- **👾 复古像素美学 (Retro Pixel Art)**
独特的 8-bit 风格 Banner 设计，搭配霓虹粉与赛博绿的配色，让原本枯燥的运维工作变得赏心悦目。
- **📊 动态流式渲染 (Live Streaming UI)**
无需等待扫描完成即可查看目录结构，数据实时跳动更新，进度条动态展示存储占用比例。
- **🎮 沉浸式交互 (Immersive Navigation)**
支持 Vim 风格按键 (`j/k/h/l`) 及标准方向键，提供丝滑的目录钻取体验。
- **🛠️ 零依赖部署 (Zero Dependencies)**
编译为单二进制文件，无需 Python 环境，无需动态库，拖入服务器即可直接运行。

## 📥 安装与构建 (Installation)

由于 **THE COVER** 是单文件工具，你可以直接下载二进制文件或从源码构建。


## 💻 使用说明 (Usage)

### 基础命令

在终端中直接运行即可扫描当前目录：

```bash
./thecover
```

也可以指定扫描特定的路径：

```bash
# 扫描根目录
./thecover /

# 扫描指定的数据盘
./thecover /data6/project
```

### ⌨️ 键盘快捷键 (Controls)

THE COVER 提供了符合直觉的键位映射：

| **按键** | **功能** | **Vim 模式** |
| --- | --- | --- |
| **↑ / ↓** | 上下移动光标 | `k` / `j` |
| **→ / Enter** | 进入选中的文件夹 | `l` |
| **← / Backspace** | 返回上一级目录 | `h` |
| **s** | **按大小排序** (Sort by size) | `s` |
| **q / Ctrl+C** | 退出软件 | `q` |

## 🛠️ 技术栈 (Tech Stack)

- **Language:** Golang
- **TUI Framework:** [Bubble Tea](https://github.com/charmbracelet/bubbletea)
- **Styling:** [Lip Gloss](https://github.com/charmbracelet/lipgloss)

