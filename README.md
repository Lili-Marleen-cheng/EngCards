# EngCards

# README.md

# 📚 背单词（CET4 / CET6 Vocabulary Learning App）

> 一个移动端优先的四六级背单词应用，专注于高效记忆、轻量学习与本地数据管理。

![Platform](https://img.shields.io/badge/Platform-Web-blue)
![Mobile First](https://img.shields.io/badge/Design-Mobile%20First-green)
![License](https://img.shields.io/badge/License-MIT-orange)

## ✨ 项目简介

**背单词** 是一款面向英语四六级考试学习者打造的轻量级单词记忆工具。

应用采用 **移动端优先设计**，提供单词卡片学习、学习进度统计、不认识单词管理、自定义词库导入导出等功能，同时支持夜间模式与本地数据持久化存储，帮助用户在碎片化时间内高效积累词汇量。

---

## 🚀 功能亮点

### 📖 单词卡片学习

* 单词卡片式学习体验
* 展示单词、音标、释义与例句
* 支持英式 / 美式发音朗读
* 一键标记：
  * ✅ 认识
  * ❌ 不认识
* 自动记录学习进度与学习统计数据

### 📊 学习数据统计

首页实时展示：


| 数据项     | 说明             |
| ---------- | ---------------- |
| 今日已学   | 当日学习数量     |
| 总单词量   | 当前词库总词数   |
| 不认识单词 | 累积待复习单词数 |

---

### 📚 多词库支持

支持三种词库：

* CET4（四级）
* CET6（六级）
* 自定义词库

用户可自由切换学习目标。

---

### 📥 自定义词库导入

支持两种导入格式：

#### 文本格式

```text
abandon,əˈbændən,v. 放弃,He abandoned his car.
ability,əˈbɪləti,n. 能力,She has the ability...
```

#### JSON 格式

```json
[
  {
    "word": "abandon",
    "phonetic_uk": "...",
    "phonetic_us": "...",
    "meaning": "...",
    "example": "..."
  }
]
```

支持：

* 替换导入
* 合并导入

并可选择导入至：

* CET4
* CET6
* 自定义词库

---

### 📤 数据导出

支持导出个人词库数据，方便备份与迁移。

---

### 📝 不认识单词管理

学习过程中标记为“不认识”的单词会自动进入复习列表。

支持：

* 查看全部待复习单词
* 快速定位学习
* 一键清空列表

---

### 🌙 夜间模式

支持明暗主题切换：

* 白天模式
* 夜间模式

自动保存用户偏好设置。

---

### 💾 本地离线存储

应用使用浏览器 LocalStorage 保存：

* 学习进度
* 词库数据
* 不认识单词列表
* 每日学习统计
* 用户设置

刷新页面后数据仍可保留。

---

## 📱 界面结构

```text
首页
 ├─ 今日学习统计
 ├─ 开始学习
 ├─ 单词列表
 ├─ 导入词库
 └─ 词库切换

单词卡片页
 ├─ 单词
 ├─ 音标
 ├─ 发音
 ├─ 释义
 ├─ 例句
 └─ 认识/不认识

不认识单词页
 └─ 错词复习

我的
 ├─ 夜间模式
 ├─ 重置学习进度
 ├─ 清空不认识单词
 ├─ 清空词库
 └─ 导出词库
```

---

## ⚡ 快速开始

### 1. 克隆项目

```bash
git clone https://github.com/your-name/word-learning-app.git
```

### 2. 进入项目目录

```bash
cd word-learning-app
```

### 3. 启动项目

直接打开：

```text
index.html
```

或使用本地服务器：

```bash
python -m http.server 8080
```

访问：

```text
http://localhost:8080
```

---

## 🏗 技术栈


| 技术               | 用途               |
| ------------------ | ------------------ |
| HTML5              | 页面结构           |
| CSS3               | UI样式与响应式布局 |
| Vanilla JavaScript | 应用逻辑           |
| LocalStorage       | 本地数据持久化     |
| Web Speech API     | 浏览器语音朗读     |
| Fetch API          | 词库加载           |

---

## 🎯 设计理念

### Mobile First

应用采用移动端优先设计：

* 手机屏幕优化布局
* 底部导航交互
* 大尺寸触控按钮
* 卡片式学习体验

### 专注学习流程

遵循：

```text
学习
 ↓
判断是否认识
 ↓
记录结果
 ↓
积累错词
 ↓
复习强化
```

降低操作成本，提高记忆效率。

---

## 📂 项目结构

```text
.
├── index.html
├── cet4_words.json
└── README.md
```

> 项目默认支持从 `cet4_words.json` 加载四级词库，当加载失败时自动回退至内置默认词库。

---

## 🔧 可扩展方向

欢迎基于项目继续扩展：

* 单词搜索
* 智能复习算法
* 学习日历
* 数据可视化
* 云端同步
* PWA离线安装
* 多语言支持

---

## 🤝 贡献指南

欢迎提交：

* Bug 修复
* 性能优化
* UI 改进
* 新功能建议
* 词库完善

贡献流程：

```bash
Fork
  ↓
Create Branch
  ↓
Commit Changes
  ↓
Push
  ↓
Pull Request
```

---

## 📄 License

本项目采用 **MIT License**。

```text
MIT License
```

---

## ⭐ 如果这个项目对你有帮助

欢迎给项目点一个 Star ⭐

你的支持将帮助项目持续改进与维护。
