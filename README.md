<div align="center">

# 🚀 DevCheatsheet / 开发者常用命令速查宝典

**精炼、实用、开箱即用的程序员日常运维与开发指令速查手册**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![Awesome](https://img.shields.io/badge/Awesome-DevCheatsheet-orange.svg?style=flat-square&logo=awesome-lists)](https://github.com/sindresorhus/awesome)[![Markdown](https://img.shields.io/badge/Format-Markdown-blue.svg)](https://commonmark.org)

[📖 阅读文档](#-目录指南) • [🛠️ 在线资源](#-在线开发者资源推荐) • [🤝 参与贡献](#-贡献指南)

</div>

---

## 📌 项目简介

在日常开发、运维及大数据处理过程中，频繁查找冗长繁琐的命令行语法往往会降低工作效率。

**DevCheatsheet** 旨在提供一份涵盖 **Linux 系统管理、后台任务调度、版本控制、Python 环境隔离、文档排版以及大数据集群** 等核心场景的高频指令与速查手册。告别谷歌搜索，助你一键查阅，高效开发！

---

## 💡 项目亮点

- ⚡ **精准高效**：剔除冷门参数，精炼最常用、最实用的命令用法。
- 📂 **分类清晰**：模块化结构设计，方便快速定位知识点。
- 🛠️ **实践导向**：附带实际场景示例与实用技巧，拒绝纸上谈兵。
- 🔗 **延伸拓展**：整合优质在线 API 手册与官方文档，一站式查阅。

---

## 📖 目录指南

点击下方链接即可直接跳转至对应的速查文档：

| 分类板块 | 文档链接 | 描述与核心内容 |
| :--- | :--- | :--- |
| 🐧 **Linux 运维** | [Linux 常用命令](./Linux常用命令.md) | 文件操作、权限管理、网络诊断、系统状态监测 |
| ⚡ **后台进程** | [nohup 指令速查](./nohup指令.md) | 后台任务挂起、日志重定向、进程管理与守护 |
| 🔀 **版本控制** | [Git 指令速查](./Git指令.md) | 分支管理、Commit 规范、撤销回滚、冲突解决 |
| 🐍 **环境管理** | [Anaconda 常用命令与技巧](./Anaconda%20常用命令与技巧.md) | 虚拟环境创建与迁移、包依赖管理、镜像加速 |
| 📝 **文档写作** | [Markdown 语法速查](./Markdown%20语法速查.md) | 基础语法、高级表格、数学公式与 Mermaid 图表 |
| 🐘 **大数据生态** | [大数据环境常用命令速查](./大数据环境常用命令速查.md) | Hadoop HDFS 命令、YARN 任务提交、Hive/Spark 交互 |

---

## 🖼️ Preview / 快速预览

### 常见场景示例

> **💡 Linux 后台不中断运行 Python 脚本并重定向日志：**
```bash
nohup python -u main.py > app.log 2>&1 &
```

> **💡 Anaconda 快速导出与重建完全相同的环境：**
```bash
# 导出当前环境
conda env export > environment.yml

# 根据文件重建环境
conda env create -f environment.yml
```

> **💡 Git 撤销上一次提交但保留修改：**
```bash
git reset --soft HEAD~1
```

---

## 🌐 在线开发者资源推荐
除了本仓库整理的本地速查手册外，以下优质的在线文档与 API 手册能为你提供更深度的参考：

🛠️ Linux 综合参考

- [Linux 命令大全 (菜鸟教程)](https://www.runoob.com/linux/linux-command-manual.html) — 适合快速检索具体命令参数

- [Linux API 速查手册 (BookStack)](https://www.bookstack.cn/read/linuxapi/docs-open.md) — 适合 C/C++ 开发者查询系统调用

- [Linux System Programming (Man Pages Section 2)](https://www.man7.org/linux/man-pages/dir_section_2.html) — Linux 官方权威 API 手册

⚙️ 构建与自动化工具

[CMake 官方教程 (中文版)](https://cmake-doc.readthedocs.io/zh-cn/latest/guide/tutorial/index.html) — C/C++ 项目构建必备指南

🐘 大数据生态

[Apache Hadoop 官方文档](https://hadoop.apache.org/docs/stable/) — HDFS & YARN 权威指南

---

## 🗺️ Roadmap / 未来规划
- [x] 完成基础模块整理（Linux, Git, Anaconda, Markdown, Hadoop）

- [x] 补充 nohup 及后台任务管理专门文档

- [ ] 增加 Docker & Kubernetes (k8s) 常用命令速查

- [ ] 增加 SQL / MySQL / Redis 高频指令集

- [ ] 增加 Shell 脚本编写百宝箱 (常用的 Bash 实用函数)

- [ ] 提供 PDF / EPUB 离线下载版

---

## 🤝 贡献指南 (Contributing)
非常欢迎你为这个项目做出贡献！如果你发现了错别字、命令参数错误，或者想添加新的实用速查模块：

1. Fork 本仓库

2. 创建你的特性分支 (git checkout -b feature/AmazingCheat)

3. 提交你的修改 (git commit -m 'Add some AmazingCheat')

4. 推送到分支 (git push origin feature/AmazingCheat)

5. 发起一个 Pull Request

---

## 📄 License & 致谢
本项目采用 [MIT License](https://www.google.com/search?q=LICENSE) 开源协议。

特别感谢以下开源社区与文档对本项目的启发：

- [Runoob (菜鸟教程)](https://www.runoob.com/)

- [man7.org](https://www.man7.org/)

- 所有致力于知识共享的开源贡献者们！
