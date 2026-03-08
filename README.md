# 华中农业大学本科生毕业论文 LaTeX 模板

<p align="center">
  <img src="https://img.shields.io/badge/HZAU-毕业论文模板-green" alt="HZAU">
  <img src="https://img.shields.io/badge/LaTeX-XeLaTeX-blue" alt="LaTeX">
  <img src="https://img.shields.io/badge/心河Paper-在线支持-orange" alt="心河Paper">
</p>

> 🎓 一份符合华中农业大学本科生毕业论文格式要求的 LaTeX 模板

## 📋 项目简介

本项目是基于 [eriche2016/HZAU_UnderGraduateThesis_Template](https://github.com/eriche2016/HZAU_UnderGraduateThesis_Template) 进行二次开发的华中农业大学本科生毕业论文 LaTeX 模板。

感谢原作者的出色工作，本模板在此基础上进行了优化和扩展，旨在帮助华中农业大学的本科生更加规范、高效、美观地撰写毕业设计论文。

## ✨ 模板特性

- ✅ **完全符合学校规范** — 遵循华中农业大学最新本科生毕业论文格式要求
- ✅ **完整封面与声明** — 自动生成中文封面、英文封面、原创性声明
- ✅ **规范排版** — 标准页眉页脚、章节格式、参考文献格式（GB/T 7714-2015）
- ✅ **双语支持** — 完善的中英文摘要、图表双标题支持
- ✅ **即开即用** — 清晰的项目结构，简单易用的命令
- ✅ **持续维护** — 根据每年毕业论文要求持续更新

## 🚀 使用方式

### 方式一：心河Paper 在线编辑（推荐）

访问 [**paper.huimengxinhe.com**](https://paper.huimengxinhe.com) 即可在线使用该模板，无需配置本地环境：

- 云端编译，实时预览
- 自动保存，版本管理
- 协作编辑，多人共享

### 方式二：本地使用

#### 1. 下载模板

```bash
git clone https://github.com/your-repo/HZAU_TEMPLATE.git
cd HZAU_TEMPLATE
```

或直接下载 ZIP 文件并解压。

#### 2. 配置环境

- 安装 TeX Live（推荐 2023 或更新版本）或 MiKTeX
- 安装 VSCode + LaTeX Workshop 插件（推荐）
- 或使用 Overleaf 在线编辑

> ⚠️ **注意**：建议使用 XeLaTeX 或 LuaLaTeX 编译引擎以确保中文排版正确。

#### 3. 开始编写

1. 打开 `main.tex` 主文件
2. 修改个人信息（论文题目、作者、导师等）
3. 在 `chapters/` 目录下编写各章节内容
4. 在 `references.bib` 中添加参考文献
5. 编译生成 PDF

## 📁 目录结构

```
HZAU_TEMPLATE/
├── main.tex              # 主文件（论文入口）
├── HZAU.cls              # 模板类文件（定义格式）
├── references.bib        # 参考文献数据库
├── latexmkrc             # LaTeX 编译配置
├── chapters/             # 论文章节目录
│   ├── chapter1.tex      # 第一章：绪论
│   ├── chapter2.tex      # 第二章：文献综述
│   ├── chapter3.tex      # 第三章：材料与方法
│   ├── chapter4.tex      # 第四章：结果与讨论
│   ├── chapter5.tex      # 第五章：结论
│   └── appendix.tex      # 附录
├── Fig/                  # 图片资源目录
│   ├── author_signature.png    # 作者签名
│   └── mentor_signature.png    # 导师签名
└── README.md             # 项目说明
```

## 📝 快速开始指南

### 修改个人信息

在 `main.tex` 中找到以下命令并修改为个人信息：

```latex
% 论文题目
\newcommand{\thesisTitleC}{你的中文论文题目}
\newcommand{\thesisTitleE}{Your English Thesis Title}

% 个人信息
\newcommand{\yourMajor}{你的专业}
\newcommand{\yourName}{你的姓名}
\newcommand{\yourMentor}{导师姓名}
\newcommand{\Mentorjob}{导师职称}
\newcommand{\studentID}{你的学号}
\newcommand{\yourClass}{你的班级}
```

### 添加签名（重要！）

提交最终版本时，请将导师签名和个人签名图片放置在 `Fig/` 目录下：

```latex
\newcommand{\authorSignature}{Fig/author_signature.png}
\newcommand{\mentorSignature}{Fig/mentor_signature.png}
```

### 编写章节

在 `chapters/` 目录下的各 `.tex` 文件中编写内容，使用 `\input{chapters/chapter1}` 引入主文件。

### 管理参考文献

使用 `\citep{key}` 命令引用文献（注意：使用 citep 而非 cite），所有文献条目维护在 `references.bib` 文件中。

## 🛠️ 编译说明

推荐使用以下方式编译：

```bash
# 使用 latexmk（推荐）
latexmk -xelatex main.tex

# 或手动编译
xelatex main.tex
biber main
xelatex main.tex
xelatex main.tex
```

## 🤝 致谢

- 感谢原作者 [**eriche2016**](https://github.com/eriche2016) 提供的 [HZAU_UnderGraduateThesis_Template](https://github.com/eriche2016/HZAU_UnderGraduateThesis_Template) 基础模板
- 感谢 [**心河Paper**](https://paper.huimengxinhe.com) 平台提供的在线编辑支持

## 🔄 更新日志

| 日期 | 版本 | 更新内容 |
|------|------|----------|
| 2025-06 | v1.0 | 初始版本发布，适配 2025 届毕业论文要求 |

> 💡 **持续维护承诺**：本模板将根据华中农业大学每年毕业论文格式要求的更新进行持续维护和优化，建议关注仓库获取最新版本。

## 📧 反馈与支持

如在使用过程中遇到问题，欢迎通过以下方式反馈：

- 提交 [GitHub Issue](../../issues)
- 联系维护者邮箱：xwhe@mail.hzau.edu.cn

反馈时请提供：
- 错误信息截图
- 操作系统和 TeX 发行版版本
- 复现步骤

## 📜 版权声明

本模板仅供华中农业大学本科生学术使用，请遵守学校相关规定。

---

<p align="center">
  <strong>祝您论文撰写顺利，毕业快乐！</strong> 🎓✨
</p>

<p align="center">
  <em>最后更新：2025年6月</em>
</p>
