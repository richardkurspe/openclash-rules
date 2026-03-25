# 🚀 OpenClash 去广告规则集

> 🎯 一个专为 **OpenClash / Clash.Meta** 打造的高效去广告规则集合  
> 📦 精简、稳定、低延迟、持续更新  

---

## 📌 项目简介

本项目维护了一套适用于 **OpenClash / Clash.Meta** 的去广告规则，主要目标是：

- 🚫 屏蔽常见海外广告域名（App / Web / 跟踪器）
- ⚡ 完美适配OpenClash格式
- 🧠 避免误杀（兼顾可用性）
- 🔄 持续更新 & 优化

适用于：

- OpenClash（ImmortalWrt / OpenWrt）
- Clash.Meta
- Mihomo 内核

---

## ✨ 特性亮点

- 📉 **轻量级设计**：相比传统广告规则更精简
- 🧩 **多源整合**：融合多个高质量规则源
- 🛠 **手动筛选优化**：去除无效 / 过时 / 高误杀条目
- 🔍 **针对国内环境优化**
- 🧪 **长期实测稳定**

---

## 📥 使用方法

### 1️⃣ 远程订阅方式（推荐）

在 OpenClash 中添加规则提供者：

```yaml
rule-providers:
  adblock:
    type: http
    behavior: domain
    url: https://你的仓库地址/ad.list
    path: ./ruleset/ad.yaml
    interval: 86400