# 🚀 OpenClash 常见规则集

> 🎯 一个专为 **OpenClash / Clash.Meta** 打造的高效规则集,内含去广告规则&附加代理规则&直连规则&特殊网站分流规则等等,一个项目全搞定！ 
>
> 📦 精简、稳定、低延迟、持续更新  

---

## 📌 项目简介

| Name | Description | Required | Default |
|------|-------------|----------|--------|
|      |             |          |        |
|      |             |          |        |
|      |             |          |        |
|      |             |          |        |
|      |             |          |        |

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

## 🗺 目录

- [特性亮点](#-特性亮点)
- [使用方法](#-使用方法)

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
  adblock:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/richardkurspe/openclash-rules/main/rule.yaml
    path: ./ruleset/ad.yaml
    interval: 86400