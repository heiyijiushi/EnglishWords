# EnglishWords - 程序员单词本

<div align="center">

**一个帮助程序员系统学习和掌握技术英文单词的开源学习平台**

[English](#english) | [中文](#中文)

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Stars](https://img.shields.io/github/stars/heiyijiushi/EnglishWords.svg)
![Contributors](https://img.shields.io/github/contributors/heiyijiushi/EnglishWords.svg)

</div>

---

## 中文

### 📌 项目简介

**EnglishWords** 是一个开源项目，旨在为中文程序员提供系统高效的技术英文学习工具。

核心目标：
- 📚 **积累词汇** - 收集和整理与编程相关的英文单词和术语
- 🎯 **高效学习** - 通过智能复习算法提高学习效率
- 📊 **跟踪进度** - 详细的学习统计和进度可视化
- 🌐 **开源社区** - 欢迎社区贡献和改进

### 🌟 主要功能

- ✅ **丰富的单词库** - 分类整理的编程相关英文单词
- ✅ **互动学习** - 卡片学习、拼写练习、听音选择等多种学习模式
- ✅ **智能复习** - 基于遗忘曲线的复习提醒机制
- ✅ **学习测验** - 自定义测验，实时评分反馈
- ✅ **进度统计** - 详细的学习数据和进度分析
- ✅ **多设备支持** - 在Web和移动设备上无缝学习

### 🚀 快速开始

#### 1. 了解项目

```bash
# 克隆仓库
git clone https://github.com/heiyijiushi/EnglishWords.git
cd EnglishWords

# 阅读项目分析文档
cat PROJECT_ANALYSIS.md

# 查看开发路线图
cat DEVELOPMENT_ROADMAP.md

# 快速启动指南
cat QUICKSTART.md
```

#### 2. 设置开发环境

详见：[快速开始指南](./QUICKSTART.md#-立即可行的任务优先级从高到低)

#### 3. 启动开发

```bash
# 后端
cd backend
npm install
npm run dev

# 前端（新终端窗口）
cd frontend
npm install
npm run dev
```

### 📚 文档

- [📖 项目分析](./PROJECT_ANALYSIS.md) - 深入了解项目目标、现状和技术分析
- [🗺️ 开发路线图](./DEVELOPMENT_ROADMAP.md) - 详细的分阶段开发计划和建议
- [⚡ 快速开始](./QUICKSTART.md) - 最快上手项目的指南
- [🤝 贡献指南](./CONTRIBUTING.md) - 如何为项目做出贡献
- [📝 API文档](./docs/API_SPECIFICATION.md) - API接口详细说明（待完成）
- [💾 数据库设计](./docs/DATABASE_SCHEMA.md) - 数据库模式和设计（待完成）

### 💻 技术栈

| 技术层 | 推荐技术 | 备选方案 |
|-------|--------|--------|
| 前端 | React 18 + Tailwind CSS | Vue 3, Svelte |
| 后端 | Nest.js (Node.js) | FastAPI (Python), Express |
| 数据库 | PostgreSQL | MySQL, MongoDB |
| ORM | Prisma | TypeORM, SQLAlchemy |
| 部署 | Docker + GitHub Actions | K8s, GitLab CI |

更详细的技术栈说明见：[开发路线图 - 技术栈](./DEVELOPMENT_ROADMAP.md#11-确定技术栈--优先级极高)

### 📁 项目结构

```
EnglishWords/
├── docs/                       # 项目文档
│   ├── PROJECT_ANALYSIS.md    # 项目分析
│   ├── DEVELOPMENT_ROADMAP.md # 开发路线图
│   ├── API_SPECIFICATION.md   # API规范（待完成）
│   └── DATABASE_SCHEMA.md     # 数据库设计（待完成）
├── data/                       # 数据文件
│   └── words/                 # 单词库
│       ├── beginner.json      # 初级单词
│       ├── intermediate.json  # 中级单词
│       └── advanced.json      # 高级单词
├── backend/                    # 后端代码（待完成）
├── frontend/                   # 前端代码（待完成）
├── README.md                   # 项目说明（本文件）
├── QUICKSTART.md               # 快速开始指南
├── CONTRIBUTING.md             # 贡献指南
├── .gitignore                  # Git忽略配置
└── LICENSE                     # MIT许可证
```

### 🤝 参与贡献

我们热烈欢迎所有形式的贡献！

**贡献方式：**
- 🐛 [报告Bug](./CONTRIBUTING.md#报告bug)
- ✨ [提出功能建议](./CONTRIBUTING.md#功能建议)
- 💻 [提交代码](./CONTRIBUTING.md#提交pr流程)
- 📝 [改进文档](./CONTRIBUTING.md#开发环境设置)
- 📚 [扩展词库](./data/words/)

详见：[完整贡献指南](./CONTRIBUTING.md)

### 📊 项目现状

- 🎉 **阶段**：初始构建阶段
- 📋 **文档**：项目分析、路线图、快速指南已完成
- 🔧 **框架**：待选择和初始化
- 💼 **功能**：待开发

### 🎯 下一步

1. **确定技术栈** - 选择最适合的前后端框架
2. **搭建基础框架** - 初始化项目代码库
3. **开发核心功能** - 实现认证、单词、学习等核心模块
4. **上线部署** - 选择合适的云平台部署
5. **社区运营** - 邀请用户和贡献者参与

详见：[开发路线图](./DEVELOPMENT_ROADMAP.md)

### 📬 联系方式

- GitHub Issues：[提问和讨论](../../issues)
- GitHub Discussions：[社区讨论](../../discussions)
- Email：heiyijiushi@example.com (示例)

### 📄 许可证

本项目采用 [MIT许可证](./LICENSE) - 详见LICENSE文件

### ✨ 致谢

感谢所有为这个项目做出贡献的开发者和使用者！🙌

---

## English

### 📌 About

**EnglishWords** is an open-source learning platform designed to help Chinese programmers systematically learn and master technical English words.

### 🌟 Features

- 📚 Rich word database with programming-related vocabulary
- 🎯 Multiple learning modes (flashcards, spelling, listening, etc.)
- 📊 Progress tracking and statistics
- 🔄 Spaced repetition algorithm for optimal learning
- 📱 Multi-device support

### 🚀 Quick Start

```bash
# Clone repository
git clone https://github.com/heiyijiushi/EnglishWords.git
cd EnglishWords

# Read documentation
cat PROJECT_ANALYSIS.md
cat DEVELOPMENT_ROADMAP.md
cat QUICKSTART.md
```

### 📚 Documentation

- [Project Analysis](./PROJECT_ANALYSIS.md)
- [Development Roadmap](./DEVELOPMENT_ROADMAP.md)
- [Quick Start](./QUICKSTART.md)
- [Contributing Guide](./CONTRIBUTING.md)

### 💻 Tech Stack

- Frontend: React 18 + Tailwind CSS
- Backend: Nest.js (Node.js)
- Database: PostgreSQL
- Deployment: Docker + GitHub Actions

### 📄 License

MIT - See [LICENSE](./LICENSE) file

---

**更新时间：2024年**

**项目版本：v0.1（初始阶段）**
