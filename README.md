# 旧版本、废弃备用版
# 一、项目介绍

## 核心

- Xray-core
- sing-box

## 协议

> 以下均使用TLS，支持多种协议组合

- VLESS(Reality、Vision(TCP)、WS、gRPC)
- VMess(TCP、WS、HTTPUpgrade)
- Trojan(TCP、gRPC)
- Hysteria2(sing-box)
- Tuic(sing-box)
- NaiveProxy(sing-box)

## 功能

- 支持不同核心之间的配置读取
- 支持个性化安装单个协议
- [支持无域名版本的VLESS Reality搭建]
- [支持多种分流用于解锁（wireguard、IPv6、Socks5、DNS、VMess(ws)、SNI反向代理）]
- [支持批量添加CDN节点并配合ClashMeta自动优选]
- 支持普通证书和通配符证书自动申请及更新
- [支持订阅以及多VPS组合订阅]
- 支持批量新增端口[仅支持Xray-core]
- 支持核心的升级以及回退
- 支持自主更换伪装站点
- 支持BT下载管理以及域名黑名单管理
- 指定默认安装Xray-core的版本为:1.7.5（需要新版本可以安装后自行升级Xray-core）



# 二、安装使用

## 1.下载脚本

- 支持快捷方式启动，安装完毕后，shell输入【**sinian**】即可打开脚本，脚本执行路径[**/etc/v2ray-agent/install.sh**]

- Github
```
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/sinian-liu/v2ray-agent/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
```
