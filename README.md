# 医学统计与生物信息学习平台 | Medical Statistics & Bioinformatics Learning Platform

[![GitHub Pages](https://img.shields.io/badge/deployed-GitHub%20Pages-blue)](https://ablikimeli.github.io/)
[![Version](https://img.shields.io/badge/version-3.0.0-teal)](https://ablikimeli.github.io/)

> 医学科研一站式学习平台 | One-stop platform for medical research and statistics
>
> **让医学科研更简单，让统计方法更易懂**

---

## 📖 平台介绍 | Platform Introduction

**中文**：这是一个一站式医学科研学习平台，整合了医学统计、生物信息学、临床研究、量表评估、公共数据库、科研工具等全流程的科研资源，为医学科研工作者提供全面的学习和工具支持。平台所有外部链接均为国内可正常访问的权威资源。v3.0 新增公众号60篇教程合集、中英文双语切换、移动端滑入菜单等特性。

**English**: A one-stop platform for medical research and statistics, integrating medical statistics, bioinformatics, clinical research, assessment scales, public databases, and research tools. v3.0 adds 60 WeChat tutorial articles, bilingual (Chinese/English) toggle, mobile slide-in menu, and more.

---

## ✨ 功能特性 | Features

### 完整统计方法教程 | Comprehensive Statistics Tutorials

| 中文 | English |
|------|---------|
| 从基础t检验到高级回归、贝叶斯统计、Meta分析 | From basic t-tests to advanced regression, Bayesian statistics, Meta analysis |
| 每个方法：概念简介 + SPSS操作 + R代码 + Python代码 + 案例解读 | Each method: concept intro + SPSS steps + R code + Python code + case studies |
| 缺失数据处理(MICE)、时间序列(ARIMA)、竞争风险模型 | Missing data (MICE), time series (ARIMA), competing risks |

### 60篇公众号教程合集 | 60 WeChat Tutorial Articles

**中文**：Abel医研统计公众号26周系统性教程，覆盖从基础到前沿的60篇医学统计方法文章，按4个阶段组织：权威重建期、深度强化期、前沿拓展期、品牌沉淀期。每篇文章包含完整的中文解读和R/Python代码实现。

**English**: A 26-week systematic tutorial series with 60 articles covering medical statistics from basics to advanced topics, organized in 4 phases: Foundation, Deep Dive, Advanced, and Consolidation.

### 中英文双语切换 | Bilingual Toggle

**中文**：一键切换中英文界面，导航、横幅、数据资源、量表、页脚等全部区域同步切换，TOC侧边栏也支持双语。

**English**: One-click toggle between Chinese and English, covering navigation, banner, data resources, scales, footer, and TOC sidebar.

### 移动端滑入菜单 | Slide-in Mobile Menu

**中文**：移动端自动显示汉堡菜单按钮，点击从右侧滑入导航面板，支持所有功能入口，含语言切换按钮。

**English**: Auto-displays hamburger button on mobile; click to slide in navigation panel with all feature entries and language toggle.

### 更多核心功能 | More Core Features

| 类别 | Category | 详情 | Details |
|------|----------|------|---------|
| 统计公式速查 | Formula Reference | 9个核心公式及使用条件 | 9 core formulas with conditions |
| 报告规范检查清单 | Reporting Checklists | STROBE/CONSORT/PRISMA/STARD/TRIPOD等 | 10+ checklists |
| 医学期刊统计要求 | Journal Requirements | NEJM/JAMA/Lancet/BMJ统计规范 | Top journal guidelines |
| 常见统计错误避坑 | Common Mistakes | 10个P值相关错误及正确做法 | 10 P-value pitfalls with fixes |
| 生物信息学分析 | Bioinformatics | 差异表达/富集分析/WGCNA/单细胞 | DE/Enrichment/WGCNA/scRNA |
| 医学量表汇总 | Medical Scales | 20+常用量表含信效度代码 | 20+ scales with reliability code |
| 传染病建模 | Epidemic Modeling | SEIR/SIR/SEIRS模型+Python代码 | SEIR/SIR/SEIRS + Python code |
| 公共数据库 | Public Databases | WHO/CDC/MIMIC/UK Biobank/TCGA等 | Global databases |
| 科研工具合集 | Research Tools | 文献下载/统计软件/选刊/作图 | Literature/Stats/Journal/Gráficos |
| AI科研工具 | AI Tools | ChatGPT/Claude/Elicit/Copilot等 | AI for research |
| R语言实操案例 | R Case Studies | t检验/Logistic回归/生存分析/Meta/PSM | t-test/Logistic/Survival/Meta/PSM |
| 统计决策树 | Decision Tree | 交互式按数据类型推荐方法 | Interactive method recommender |
| 深色模式 | Dark Mode | 跟随系统或手动切换 | System-aware/manual toggle |
| 全站搜索 | Full-text Search | Ctrl+K 搜索所有内容 | Ctrl+K to search everything |

---

## 🚀 快速开始 | Quick Start

1. **在线访问 | Online**: [ablikimeli.github.io](https://ablikimeli.github.io/)
2. **本地运行 | Local**: 直接打开 `index.html` 或在任意HTTP服务器中部署 | Open `index.html` directly or deploy on any HTTP server
3. **搜索 | Search**: `Ctrl+K` 或点击搜索图标 | or click search icon
4. **语言切换 | Language**: 点击右上角 `中/EN` 按钮 | Click `中/EN` button in header
5. **移动端 | Mobile**: 点击左上角 `☰` 打开导航菜单 | Tap `☰` to open navigation

---

## 📂 项目结构 | Project Structure

```text
ablikimeli_website/
├── index.html            # 主页面 (单页应用) | Main SPA
├── articles-data.js      # 60篇公众号教程数据 | 60 WeChat articles data
├── README.md             # 本文件 | This file
├── figures/              # 统计图表图片 | Statistics figures
│   └── *.png             # 33张发表级图表 | 33 publication-grade figures
└── .nojekyll             # GitHub Pages配置 | GitHub Pages config
```

数据预处理脚本 | Preprocessing script:

```text
abel_stat_wechat/scripts/
├── convert_articles_to_js.py   # Markdown → HTML → JS 转换 | Article conversion
└── apply_v3_changes.py         # index.html v3.0 修改脚本 | HTML modification
```

---

## 📅 更新日志 | Changelog

### v3.0.0 (2026-04-30)

**中文**：
- 📱 集成公众号60篇教程文章，按4个阶段组织
- 🌐 中英文双语界面切换（导航、数据、量表、侧边栏全覆盖）
- 🍔 移动端汉堡菜单 + 右侧滑入导航面板
- 🔍 文章内容纳入全站搜索
- 🐛 修复：搜索点击文章跳转、TOC双语、代码复制按钮文字硬编码
- 📖 README 中英双语重写

**English**：
- 📱 Integrated 60 WeChat tutorial articles in 4 phases
- 🌐 Bilingual UI toggle (Chinese/English) with full coverage
- 🍔 Mobile hamburger menu with slide-in navigation
- 🔍 Article content included in full-text search
- 🐛 Fixed: article search navigation, TOC bilingual support, hardcoded button texts
- 📖 Bilingual README rewrite

### v2.1.0 (2026-04-30)
- ✅ 新增研究报告规范检查清单（STROBE/CONSORT/PRISMA/STARD等10项）
- ✅ 新增主要医学期刊统计要求（NEJM/JAMA/Lancet/BMJ/Nature Med等）
- ✅ 新增常见统计错误与避坑指南
- ✅ 新增统计公式速查表（9个核心公式及使用条件）
- ✅ 修复ChiPlot链接、RECORD链接

### v2.0.0 (2026-04-11)
- ✅ 修复统计方法按钮冲突问题
- ✅ 大幅补充量表内容，新增10+常用量表
- ✅ 移除左侧侧边导航，优化页面布局

### v1.0.0 (2026-04-10)
- ✅ 完成平台基础框架搭建
- ✅ 整合统计方法、生物信息学、数据库、工具等模块

---

## 📞 联系方式 | Contact

- **微信公众号 | WeChat Official Account**: Abel医研统计
- **平台宗旨 | Mission**: 让医学科研更简单，让统计方法更易懂 | Making medical research statistics accessible to all
- **GitHub**: [ablikimeli](https://github.com/ablikimeli)

---

## 📝 说明 | Notes

**中文**：本平台所有资源均整理自公开的权威资源，仅供学习和科研使用。如果您有任何问题或建议，欢迎通过公众号联系我们。

**English**: All resources are curated from publicly available authoritative sources for educational and research purposes only. Feel free to contact us via WeChat with any questions or suggestions.
