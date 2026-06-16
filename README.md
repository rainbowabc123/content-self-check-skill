# Content Self-Check Skill

[中文](#中文文档) | [English](#english-documentation)

---

## 中文文档

### 📋 简介

**Content Self-Check** 是一个专业的自媒体文案质量自检工具，帮助内容创作者发现文案中影响阅读体验和内容质量的问题。

这是一个 AI Skill，可以集成到 Claude Code、Anthropic API 或其他 AI 助手中使用。

### ✨ 核心功能

- ✅ **10 项质量检测**：语病、逻辑断层、数字错误、引用错误、事实一致性、排版规范、专业术语、情绪断层、标题匹配度、信息完整性
- 🎯 **智能分级**：按严重程度分为 🔴 严重问题、⚠️ 中等问题、💡 建议优化
- 📝 **详细报告**：每个问题都引用原文、说明理由、给出修改建议
- 🔍 **体裁识别**：自动识别小红书、公众号、短视频等不同体裁，调整检测标准
- 🤝 **尊重风格**：只改错误，不改风格，保持作者表达习惯

### 🚀 快速开始

#### 安装方法

**方式 1：手动安装**

1. 下载 `SKILL.md` 文件
2. 放到你的 AI 助手的 skills 目录：
   - Claude Code: `.claude/skills/content-self-check/SKILL.md`
   - 或其他支持 skill 的 AI 系统

**方式 2：克隆仓库**

```bash
git clone https://github.com/YOUR_USERNAME/content-self-check-skill.git
cd content-self-check-skill
```

#### 使用方法

在 Claude Code 或支持的 AI 助手中：

```
/content-self-check

或者直接说：
"帮我检查一下这段文案"
"有没有什么问题"
```

然后粘贴你的文案即可。

### 📊 检测项目

| 检测项 | 严重度 | 说明 |
|--------|--------|------|
| 1️⃣ 语病检测 | 🔴 | 主谓宾残缺、语序混乱、歧义句式、搭配不当 |
| 2️⃣ 逻辑断层 | 🔴/⚠️ | 前后矛盾、因果不成立、推理跳跃 |
| 3️⃣ 数字错误 | 🔴 | 前后不一致、计算错误、单位错误 |
| 4️⃣ 引用错误 | 🔴/⚠️ | 来源不明、张冠李戴、引用失实 |
| 5️⃣ 事实一致性 | 🔴/⚠️ | 人物、时间、地点信息前后矛盾 |
| 6️⃣ 排版规范 | 💡 | 中英文空格、标点符号、段落格式 |
| 7️⃣ 专业术语 | ⚠️/💡 | 术语错误、不统一、未解释 |
| 8️⃣ 情绪断层 | ⚠️ | 情绪突变、语气不一致 |
| 9️⃣ 标题匹配度 | 🔴/⚠️ | 标题党、标题与内容不符 |
| 🔟 信息完整性 | ⚠️ | 承诺未兑现、引用缺失 |

### 💡 使用示例

**示例 1：检测文案**

```
用户：/content-self-check

这个产品从100万用户增长到150万用户，增长率达到了150%！
我们的创始人李明（28岁）在科技界已经打拼了20年。
```

**AI 返回：**

```
# 文案质量检测报告

**检测结果：发现 2 处问题**
- 🔴 严重问题：2 处

---

## 🔴 严重问题

### 1. [数字错误] 增长率计算错误

> 从100万用户增长到150万用户，增长率达到了150%

**问题说明**：增长率计算错误。从 100 万到 150 万，增长了 50 万，
增长率应该是 50%，而不是 150%。

**建议修改**：改为"增长率达到 50%"或"增长了 50%"

### 2. [事实一致性] 年龄与工作年限矛盾

> 创始人李明（28岁）在科技界已经打拼了20年

**问题说明**：28 岁打拼 20 年意味着 8 岁就开始工作，不符合常理。

**建议修改**：核实创始人年龄或工作年限，修正其中一个数据
```

### 🎯 适用场景

- ✍️ 公众号文章发布前的最后检查
- 📱 小红书、抖音文案质量把关
- 📊 数据报告的准确性验证
- 📖 长文的逻辑连贯性检查
- 🔍 避免低级错误损害内容可信度

### 🛠️ 技术特性

- **零依赖**：纯文本 Skill 定义，无需额外安装
- **可扩展**：可以根据需求修改检测规则
- **多语言**：支持中英文文案检测
- **体裁识别**：自动适配不同内容类型

### 📝 许可证

MIT License - 可自由使用、修改和商业化

### 🤝 贡献

欢迎提交 Issue 和 Pull Request！

### 📧 联系方式

如有问题或建议，请提交 [Issue](https://github.com/YOUR_USERNAME/content-self-check-skill/issues)

---

## English Documentation

### 📋 Introduction

**Content Self-Check** is a professional content quality checker for self-media copywriting, helping content creators identify issues that affect reading experience and content quality.

This is an AI Skill that can be integrated into Claude Code, Anthropic API, or other AI assistants.

### ✨ Key Features

- ✅ **10 Quality Checks**: Grammar, logic gaps, numerical errors, citation errors, factual consistency, formatting, terminology, emotional flow, title matching, information completeness
- 🎯 **Smart Severity Levels**: 🔴 Critical, ⚠️ Medium, 💡 Suggestions
- 📝 **Detailed Reports**: Each issue includes quoted text, explanation, and revision suggestions
- 🔍 **Content Type Recognition**: Auto-detects different formats (social media, articles, videos) and adjusts standards
- 🤝 **Style-Preserving**: Fixes errors without changing personal writing style

### 🚀 Quick Start

#### Installation

**Method 1: Manual Installation**

1. Download `SKILL.md`
2. Place it in your AI assistant's skills directory:
   - Claude Code: `.claude/skills/content-self-check/SKILL.md`
   - Or other skill-compatible AI systems

**Method 2: Clone Repository**

```bash
git clone https://github.com/YOUR_USERNAME/content-self-check-skill.git
cd content-self-check-skill
```

#### Usage

In Claude Code or supported AI assistant:

```
/content-self-check

Or simply say:
"Check my content"
"Review this copy"
```

Then paste your content.

### 📊 Detection Items

| Check | Severity | Description |
|-------|----------|-------------|
| 1️⃣ Grammar | 🔴 | Subject-verb-object issues, word order, ambiguity |
| 2️⃣ Logic Gaps | 🔴/⚠️ | Contradictions, invalid causality, reasoning jumps |
| 3️⃣ Numerical Errors | 🔴 | Inconsistencies, calculation errors, unit errors |
| 4️⃣ Citation Errors | 🔴/⚠️ | Missing sources, misattribution, false claims |
| 5️⃣ Factual Consistency | 🔴/⚠️ | Character, time, location contradictions |
| 6️⃣ Formatting | 💡 | Spacing, punctuation, paragraph structure |
| 7️⃣ Terminology | ⚠️/💡 | Term errors, inconsistency, unexplained jargon |
| 8️⃣ Emotional Flow | ⚠️ | Abrupt tone shifts, inconsistent mood |
| 9️⃣ Title Matching | 🔴/⚠️ | Clickbait, title-content mismatch |
| 🔟 Information Completeness | ⚠️ | Unfulfilled promises, missing references |

### 💡 Example Usage

**Example: Content Check**

```
User: /content-self-check

Our product grew from 1M to 1.5M users, a 150% growth rate!
Our 28-year-old founder has been in tech for 20 years.
```

**AI Response:**

```
# Content Quality Report

**Detection Result: 2 Issues Found**
- 🔴 Critical Issues: 2

---

## 🔴 Critical Issues

### 1. [Numerical Error] Growth rate calculation error

> from 1M to 1.5M users, a 150% growth rate

**Issue**: Growth rate calculation is incorrect. From 1M to 1.5M is 
an increase of 0.5M, which is a 50% growth rate, not 150%.

**Suggested Fix**: Change to "50% growth rate" or "grew by 50%"

### 2. [Factual Consistency] Age vs. work experience contradiction

> 28-year-old founder has been in tech for 20 years

**Issue**: 28 years old with 20 years of experience means starting 
at age 8, which is unrealistic.

**Suggested Fix**: Verify founder's age or work experience and correct one
```

### 🎯 Use Cases

- ✍️ Final check before publishing articles
- 📱 Quality control for social media posts
- 📊 Data report accuracy verification
- 📖 Long-form content logic review
- 🔍 Avoid basic errors that damage credibility

### 🛠️ Technical Features

- **Zero Dependencies**: Plain text skill definition, no installation needed
- **Extensible**: Customize detection rules as needed
- **Multilingual**: Supports Chinese and English content
- **Format Recognition**: Auto-adapts to different content types

### 📝 License

MIT License - Free to use, modify, and commercialize

### 🤝 Contributing

Issues and Pull Requests are welcome!

### 📧 Contact

For questions or suggestions, please submit an [Issue](https://github.com/YOUR_USERNAME/content-self-check-skill/issues)

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=YOUR_USERNAME/content-self-check-skill&type=Date)](https://star-history.com/#YOUR_USERNAME/content-self-check-skill&Date)

---

**Made with ❤️ for content creators**
