# macOS 工作环境配置

> 尽量使用开源软件 尽量少装不必要软件 尽量使用自带软件

## 系统设置

- 触摸板轻触和右键: 系统偏好设置 - 触控板 - 光标与点按 - 勾选 `轻点来点按` 和 `辅助点按`（双指点按或轻点）
- 三指拖移: 系统偏好设置 - 辅助功能 - 指针控制 - 触控板选项 - 启用拖移 - 三指拖移
- 取消自动重新排列空间: 系统偏好设置 - 调度中心 - 取消勾选 `根据最近使用情况自动重新排列空间`
- Tab 键移动焦点: 系统偏好设置 - 键盘 - 快捷键 - 全键盘控制 `所有控制`

## 常见问题

- `文件已损坏` ? : 终端输入 `sudo spctl --master-disable` ，系统偏好设置 - 安全性与隐私 - 通用 - 允许 `任何来源`

## 工具安装

```shell
# 安装 Homebrew - MacOS包管理器(命令行轻松装软件)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# ==========================================
# 开发工具 (Development Tools)
# ==========================================

# Visual Studio Code - Code editing. Redefined.
brew install --cask visual-studio-code

# Cursor - An editor made for programming with AI.
brew install --cask cursor

# Antigravity - Internal Agent Application.
brew install --cask antigravity

# Android Studio - Android平台开发集成环境。
brew install --cask android-studio

# Emacs - GNU Emacs text editor (GUI version).
brew install --cask emacs-app

# Flutter - Google's UI toolkit for building natively compiled applications.
brew install --cask flutter

# IntelliJ IDEA - 强大的Java集成开发环境 (Ultimate版本)。
brew install --cask intellij-idea

# ==========================================
# 数据库与管理工具 (Database & Management Tools)
# ==========================================

# DBeaver Community - 通用数据库图形客户端。
brew install --cask dbeaver-community

# redis-insight - Redis官方可视化工具。
brew install --cask redis-insight

# ==========================================
# 笔记与知识管理 (Notes & Knowledge Management)
# ==========================================

# Obsidian - A powerful knowledge base that works on top of a local folder of plain text Markdown files.
brew install --cask obsidian

# ==========================================
# 终端与命令行 (Terminal & CLI)
# ==========================================

# tmux - Terminal multiplexer. Allows multiple sessions and window splitting in a single terminal.
brew install tmux

# Alacritty - A fast, cross-platform, OpenGL terminal emulator.
brew install --cask alacritty

# ==========================================
# 浏览器 (Browsers)
# ==========================================

# Google Chrome - 是由Google开发的免费网页浏览器。
brew install --cask google-chrome

# Firefox - Free and open-source web browser developed by the Mozilla Foundation.
brew install --cask firefox

# ==========================================
# 社交通讯 (Communication)
# ==========================================

# Telegram - a new era of messaging
brew install --cask telegram

# WeChat (微信) - 一款跨平台的通讯工具。
brew install --cask wechat

# QQ - I'm QQ - 每一天，乐在沟通。
brew install --cask qq

# Microsoft Teams - Communication and collaboration platform.
brew install --cask microsoft-teams

# LocalSend - A cross-platform file sharing app.
brew install --cask localsend

# XMind - Mind mapping and brainstorming tool.
brew install --cask xmind

# ==========================================
# 网络与系统工具 (Network & System Utilities)
# ==========================================

# OrbStack - Fast, light, and easy way to run Docker containers and Linux machines.
brew install --cask orbstack

# WinBox - MikroTik RouterOS GUI configurator.
brew install --cask winbox

# Tunnelblick - Tunnelblick是OS X和macOS上用于OpenVPN（虚拟专用网络）的免费开源图形用户界面。它提供对OpenVPN客户端和/或服务器连接的轻松控制。
brew install --cask tunnelblick

# Aerospace - An i3-like tiling window manager for macOS.
brew install --cask aerospace

# Karabiner-Elements - A powerful utility for keyboard customization on macOS.
brew install --cask karabiner-elements

# Mos - A lightweight tool used to smooth scrolling and set scroll direction independently for your mouse.
brew install --cask mos

# Tencent Lemon (腾讯柠檬清理) - 全新Mac清理工具，实时了解Mac系统状况。
brew install --cask tencent-lemon

# BetterDisplay - Display management tool (Resolution, XDR brightness, etc.).
brew install --cask betterdisplay

# Ice - Powerful menu bar manager for macOS (similar to Bartender).
brew install --cask jordanbaird-ice

# Battery Toolkit - App to manage battery charging.
brew install --cask battery-toolkit
```

## 开发相关

```shell
# 脚本安装 nvim 配置
sh <(curl -L https://github.com/zouzonghua/nvim/raw/lua/install.sh)

# 脚本安装 dotfiles 
sh <(curl -L https://github.com/zouzonghua/dotfiles/raw/main/install.sh)

# 生成 ssh key 并加入 git 账户
ssh-keygen # 一路回车即可

# 粘贴到自己 git 账号设置里的 ssh-key
cat ~/.ssh/id_rsa.pub | clipcopy

# 配置用户信息
git config --global user.name "zouzonghua"
git config --global user.email "zouzonghua.cn@gmail.com"

# 粘贴到终端配置 ssh 免密登陆服务器
ssh-copy-id -i ~/.ssh/id_rsa.pub -p 22 root@www.zouzonghua.cn
```
## 配置文件

- [dotfiles](https://github.com/zouzonghua/dotfiles)
