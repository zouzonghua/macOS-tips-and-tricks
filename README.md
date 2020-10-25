# MacOS 工作环境配置

#### 系统设置

- 触摸板轻触和右键: 系统偏好设置 - 触控板 - 光标与点按 - 勾选 `轻点来点按` 和 `辅助点按`（双指点按或轻点）
- 三指拖移: 系统偏好设置 - 辅助功能 - 指针控制 - 触控板选项 - 启用拖移 - 三指拖移
- 修改密码: 系统偏好设置 - 用户与群组 - 更改密码
- 修改用户名: 系统偏好设置 - 用户与群组 - 点击左下角解锁 - 用户名上双指轻点 - 高级选项
- 电脑改名: 系统偏好设置 - 共享 - 电脑名称
- 控制音频切换: 系统偏好设置 - 声音 - 在菜单中显示音量 
- 取消自动重新排列空间: 系统偏好设置 - 调度中心 - 取消勾选 `根据最近使用情况自动重新排列空间`

#### 常见问题

- “文件已损坏”?: 终端输入 `sudo spctl --master-disable` ，系统偏好设置 - 安全性与隐私 - 通用 - 允许“任何来源”

#### 工具安装

```shell
# 【必装】安装 Homebrew - MacOS包管理器(命令行轻松装软件)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

# 【必装】oh-my-zsh - 更强大的终端Shell
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# 【必装】brew-cask-upgrade is a command-line tool for upgrading every outdated app installed by Homebrew Cask.
brew tap buo/cask-upgrade

# 【必装】iTerm2 - 是一款完全免费的，专为Mac OS 用户打造的命令行应用。
brew cask install iterm2

# 【必装】unrar - 解压RAR工具
brew install unrar

# 【必装】AdoptOpenJDK - 是一个由OpenJDK构建，并以免费软件的形式提供社区版的 OpenJDK 二进制包。 它至少提供 4 年的免费长期支持(LTS)。 CentOS7.5和EulerOS2.8操作系统在鲲鹏生态中可以完整运行AdoptOpenJDK的全部功能。
brew cask install adoptopenjdk8

# 【必装】n - 管理多个Node版本的工具。
brew install n

# 【必装】Git - Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
brew install git

# 【必装】Node.js® - 是一个基于Chrome V8 引擎 的JavaScript 运行时。
n stable

# 【必装】 yarn - 快速、可靠、安全的依赖管理工具。
npm i -g yarn

# 【必装】MongoDB - 是一种面向文档的数据库管理系统，用C++等语言撰写而成，以解决应用程序开发社区中的大量现实问题。
brew tap mongodb/brew
brew install mongodb-community
brew services start mongodb-community

# 【必装】MySQL - MySQL 是最流行的关系型数据库管理系统，在 WEB 应用方面 MySQL 是最好的 RDBMS(Relational Database Management System：关系数据库管理系统)应用软件之一。。
brew install mysql@5.7

# 【必装】Visual Studio Code - 是一个由微软开发，同时支持Windows 、 Linux和macOS等操作系统且开放源代码的代码编辑器，它支持测试，并内置了Git 版本控制功能，同时也具有开发环境功能，例如代码补全、代码片段和代码重构等。
brew cask install visual-studio-code

# 【必备】IntelliJ IDEA - 是一种商业化销售的Java集成开发环境工具软件，由JetBrains软件公司开发，提供Apache 2.0开放式授权的社区版本以及专有软件的商业版本，开发者可选择其所需来下载使用。
brew cask install intellij-idea

# 【必备】wechatwebdevtools - 微信开发者工具，集成了公众号网页调试和小程序调试两种开发模式。
brew cask install wechatwebdevtools

# 【必装】Google Chrome - 是由Google开发的免费网页浏览器。
brew cask install google-chrome

# 【必装】腾讯柠檬清理 - 全新Mac清理工具，实时了解Mac系统状况。
brew cask install tencent-lemon

# 【必装】微信 - 一款跨平台的通讯工具。支持单人、多人参与。通过手机网络发送语音、图片、视频和文字。
brew cask install wechat

# 【必装】IINA - 一个现代的 macOS 视频播放器。
brew cask install iina

# 【必装】neteasemusic - 网易云音乐是一款专注于发现与分享的音乐产品，依托专业音乐人、DJ、好友推荐及社交功能，为用户打造全新的音乐生活。
brew cask install neteasemusic

# 【必装】Rectangle - Move and resize windows in macOS using keyboard shortcuts or snap areas.
brew cask install rectangle

# 【必装】v2rayx - V2RayX: A simple GUI for V2Ray on macOS.
brew cask install v2rayx

# 【必装】Tunnelblick - Tunnelblick是OS X和macOS上用于OpenVPN（虚拟专用网络）的免费开源图形用户界面。它提供对OpenVPN客户端和/或服务器连接的轻松控制。
brew cask install tunnelblick

# 【必装】bob - Bob 是一款 Mac 端翻译软件，翻译方式支持划词翻译和截图翻译，翻译引擎支持有道翻译、百度翻译和谷歌翻译。
brew cask install bob

# 【必装】mos - 一个用于在 MacOS 上平滑你的鼠标滚动效果或单独设置滚动方向的小工具, 让你的滚轮爽如触控板。
brew cask install mos

# 【必装】Fliqlo - 一个翻页时钟屏保。
brew cask install fliqlo

# 【必装】Typora - 是一款支持实时预览的Markdown 文本编辑器。
brew cask install typora

# 【必装】Navicat Premium 12.1.28 强大的数据库管理工具。
https://drive.google.com/open?id=1c7JPTklh0yqNj69JzqlZlf5Pqbmsse8T


```

#### 开发相关

```shell

# 生成 ssh key 并加入 git 账户
ssh-keygen # 一路回车即可

# 粘贴到自己 git 账号设置里的 ssh-key
cat ~/.ssh/id_rsa.pub | clipcopy

# 配置用户信息
git config --global user.name "zouzonghua"
git config --global user.email "zouzonghua0511@gmail.com"

# 粘贴到 iterm2 配置 ssh 免密登陆服务器
ssh-copy-id -i ~/.ssh/id_rsa.pub -p 22 root@www.zonghua.me
```


