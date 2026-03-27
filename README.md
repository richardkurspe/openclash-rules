> ⚠️ 本项目仅供学习研究使用，请勿用于商业用途

# 🚀 OpenClash 常见规则集
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Stars](https://img.shields.io/github/stars/richardkurspe/openclash-rules)
![Forks](https://img.shields.io/github/forks/richardkurspe/openclash-rules)
![Issues](https://img.shields.io/github/issues/richardkurspe/openclash-rules)
![OpenClash](https://img.shields.io/badge/OpenClash-Rules-green)
![AdBlock](https://img.shields.io/badge/AdBlock-Enabled-blue)
![Lightweight](https://img.shields.io/badge/Design-Lightweight-orange)
![Platform](https://img.shields.io/badge/Platform-OpenClash%20%7C%20Clash.Meta-blue)
![Ads Blocked](https://img.shields.io/badge/Ads-Blocked-red)
![Security](https://img.shields.io/badge/Security-Tested-green)

> 🎯 一个专为 **OpenClash / Clash.Meta** 打造的高效规则集,内含去广告规则&附加代理规则&直连规则&特殊网站分流规则等等,一个项目全搞定！ 
>
> 📦 精简、稳定、低延迟、持续更新  

---

## 🗺 目录

- [项目简介](#-项目简介)
- [文件目录](#-文件目录)
- [特性亮点](#-特性亮点)
- [使用方法](#-使用方法)
- [特别感谢](#-特别感谢)
---

## 📌 项目简介

本项目维护了一套适用于 **OpenClash / Clash.Meta** 的规则全家桶，主要目标是：

- 🚫 屏蔽常见海外广告域名（~~黄网~~ /App / Web / 新闻跟踪器）
- ⚡ 拓展代理网站列表，防止访问失败
- 🧠 特殊网站~~黄网~~列表：可充分利用低倍率节点，轻松省流量
- 🔄 持续更新 & 优化

适用于：

- OpenClash（ImmortalWrt / OpenWrt）
- Clash.Meta
- Mihomo 内核

---

## 📁 文件目录

```bash
openclash-rules/
├─ 📄LICENSE
├─ 📄READ.md          
├─ 📁Rules/              
│  ├── 📄Reject.yaml     # 去广告规则
│  ├── 📄Additional.yaml # 附加规则
│  ├── 📄Special.yaml    # 特殊规则
│  └── 📄Direct.yaml     # 直连规则
```

---

## ✨ 特性亮点

- 📉 **轻量级设计**：相比传统规则更精简,只保留必要的域名,加快匹配速度,降低内存使用
- 🧩 **多源整合**：融合多个高质量规则源
- 🛠 **手动筛选优化**：去除无效 / 过时 / 高误杀条目
- 🔍 **针对国内环境优化**
- 🧪 **长期实测稳定**

---

## 📥 使用方法

### 远程订阅方式（推荐）

在 OpenClash 中添加规则提供者：

```yaml
rule-providers:
  Reject:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/richardkurspe/openclash-rules/main/rules/Reject.yaml
    path: ./ruleset/ad.yaml
    interval: 86400

  Additional:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/richardkurspe/openclash-rules/main/rules/Additional.yaml
    path: ./ruleset/ad.yaml
    interval: 86400

  Special:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/richardkurspe/openclash-rules/main/rules/Special.yaml
    path: ./ruleset/ad.yaml
    interval: 86400

   Direct:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/richardkurspe/openclash-rules/main/rules/Direct.yaml
    path: ./ruleset/ad.yaml
    interval: 86400
```

---

## ❤️ 特别感谢

- 我们出色的用户社区
- 开源社区的启发

