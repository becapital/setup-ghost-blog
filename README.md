# Ghost 博客平台一键安装脚本

**新：** 在同一台服务器上 **安装多个博客**！只需再次运行脚本，并指定新的完整域名作为参数。

## 系统要求

一个专用服务器或虚拟专用服务器 (VPS)，**全新安装** 以下系统：   
- Ubuntu 16.04 (Xenial), 14.04 (Trusty) or 12.04 (Precise)
- Debian 8 (Jessie)
- CentOS 6 or 7

**注：** 需要至少 **512 MB** 内存。

## 安装说明

首先，更新你的系统： 运行 `apt-get update && apt-get dist-upgrade` (Ubuntu/Debian) 或者 `yum update` (CentOS) 并重启。这一步是可选的，但推荐。

#### 选择 ModSecurity 防火墙：

```
wget https://raw.githubusercontent.com/becapital/setup-ghost-blog/master/ghost-nginx-modsecurity.sh -O ghost-setup.sh
sudo bash ghost-setup.sh BLOG_FULL_DOMAIN_NAME [输入IP]
```
