# SS-Rust-Manager

[![Release](https://img.shields.io/github/v/release/shui1iao/SS-Rust-Manager?style=flat-square&color=2563eb)](https://github.com/shui1iao/SS-Rust-Manager/releases/latest)
[![Shell](https://img.shields.io/badge/Shell-Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)](ss-rust.sh)
[![Platform](https://img.shields.io/badge/Platform-Linux%20amd64%20%7C%20arm64-1e293b?style=flat-square&logo=linux&logoColor=white)](https://github.com/shui1iao/SS-Rust-Manager/releases)

**中文** | [English](README.en.md)

**轻量级 Shadowsocks-Rust 服务端一键安装与管理脚本**——专注纯 Shadowsocks 服务部署与维护，开箱即用。

## 核心特性

- **极简部署与升级**：一键安装、更新 `shadowsocks-rust` 官方核心，下载自动校验 SHA-256 完整性，更新后自动重启生效。
- **安全配置管理**：交互式配置监听端口、加密方式与高熵密钥，配置原子落盘并固定 `0600` 权限，自动输出标准 SIP002 分享链接。
- **多架构支持**：原生支持 `amd64` 与 `arm64`，兼容 Debian / Ubuntu 及 RHEL 系系统。
- **完善运维辅助**：内置 systemd 服务管理、系统时间同步检查与脚本自更新。

## 快速开始

### 方式一：短链一键运行（推荐）

```bash
bash <(curl -Ls https://ss.siaoz.si)
```

### 方式二：运行最新正式发布版

```bash
curl -fsSLO https://github.com/shui1iao/SS-Rust-Manager/releases/latest/download/ss-rust.sh
bash ss-rust.sh
```

## 注意事项

- 请在可信 Linux VPS 上以 `root` 身份执行。
- 仅管理 Shadowsocks-Rust 本身，不包含 ShadowTLS 或其他无关组件。
