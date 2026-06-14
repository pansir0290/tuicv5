# TUIC v5 一键部署脚本

这是一个专为 Linux VPS 设计的 **TUIC v5 快速部署脚本**。它能够自动探测你现有的 Xray/Reality 伪装环境，复用证书与域名配置，帮你快速搭建一个高抗丢包的 TUIC v5 节点。

## 🚀 功能特点

* **自动探测：** 自动寻找系统内已有的 Let's Encrypt 证书及 Xray Reality 伪装域名。
* **安全随机：** 自动生成高强度 UUID 和 Token，确保连接安全。
* **环境自适应：** 如果自动探测失败，提供交互式手动输入接口，避免安装中断。
* **一键集成：** 自动配置 systemd 守护进程，支持重启自启。
* **QoS 优化：** 内置 BBR 拥塞控制支持及包丢失预防（Packet Loss Prevention）选项。

## 📋 快速使用指南

1. **登录你的 VPS**，运行以下命令下载并安装：

```bash
sudo curl -fsSL [https://raw.githubusercontent.com/pansir0290/nginx-stream-manager/main/deploy.sh](https://raw.githubusercontent.com/pansir0290/tuicv5/main/tuic_install.sh) | bash
