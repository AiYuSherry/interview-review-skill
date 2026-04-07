# Interview Recorder Skill

[English](#english) | [中文](#中文)

---

<a name="中文"></a>
## 中文

面试录音整理 Skill - 自动化生成面试复盘文档

### 简介

面试完最浪费时间的事不是面试本身，是复盘。

这个 Skill 帮你把面试录音转写文本自动整理成三份文档：
- **面试总复盘表**：横版表格，问题+回答+亮点+改进建议+参考话术
- **面试问题总结**：按环节分类的问题清单
- **完整录音整理**：校对后的对话记录

整个过程 5 分钟，不用自己听录音、不用手动记笔记。

### 使用方法

#### 1. 安装 Skill

**方式一：GitHub 链接（推荐）**

直接把 GitHub 链接丢给任意 Agent：
```
https://github.com/AiYuSherry/interview-recorder
```

Agent 会自动下载并安装 skill。

**方式二：手动安装**

把 `interview-recorder.md` 文件放到你的 Agent skills 目录：

```bash
# Claude Code
~/.claude/skills/interview-recorder.md

# 其他 Agent 工具
# 放到对应的 skills 文件夹
```

#### 2. 准备面试录音

推荐使用 **腾讯元宝 AI 录音笔** 录制面试：
- 转写准确率高
- 支持实时转写
- 免费使用

其他备选：讯飞听见、飞书妙记、通义听悟

#### 3. 生成复盘文档

把录音转写后的文本发给 Agent，说出关键词即可触发：

> "帮我整理这个面试录音"
> 
> "面试复盘"
> 
> "这是今天的面试记录"

Agent 会自动输出三个 Word 文档，存放在统一命名的文件夹中。

### 输出文件结构

```
面试复盘-{公司}-{部门}-{日期}/
├── 1-面试总复盘-{公司}-{部门}-{日期}.docx      # 横版表格
├── 2-面试问题总结-{公司}-{部门}-{日期}.docx    # 竖版问题清单
└── 3-面试录音整理-{公司}-{部门}-{日期}.docx    # 校对后的完整记录
```

#### 文档1：面试总复盘

横版 A4 表格，包含：
| 序号 | 面试问题 | 我的回答摘要 | 回答亮点 | 改进建议 | 参考话术 |
|:---:|:---|:---|:---|:---|:---|

- **我的回答摘要**：提炼核心要点，不逐字复述
- **回答亮点**：肯定做得好的地方
- **改进建议**：具体可执行的优化方向
- **参考话术**：优化后的回答示例

#### 文档2：面试问题总结

按环节分类的问题清单：
- 开场/英文能力测试
- 求职动机与准备
- 过往经历深挖
- 专业知识考察
- 职业规划
- 时间安排
- 反问环节

追问使用子编号（1.1, 1.2）

#### 文档3：完整录音整理

按主题分段的对话记录：
- 修正语音识别错误
- 规范英文转写
- 补充专业术语全称
- 删除语气词和重复词

### 格式规范

- **汉字**：楷体
- **英文/数字**：Times New Roman
- **标题**：16pt / 14pt
- **正文**：10.5pt
- **复盘表**：横版 A4，9pt 字号

### 为什么这样做

**不想重复踩坑**

面试里很多问题都是高频出现的。第一次答得磕磕绊绊，如果不去整理，第二次可能还是原样。但如果有一个地方专门记录"这个问题我上次是怎么答的、哪里该改"，下次面试前翻一眼，效果就好很多。

**避免混淆**

面多了会记不清"这家问了我什么、那家问了什么"。每个面试独立存档，想查什么随时能查。

**节省时间**

与其花一两小时听录音、记笔记，不如 5 分钟让 AI 整理成能复用的东西。

---

<a name="english"></a>
## English

Interview Recorder Skill - Automatically generate interview review documents from transcript

### Introduction

The most time-consuming part of an interview isn't the interview itself—it's the review afterward.

You've been there: a 40-minute interview recording sits in your folder for two weeks because you don't have the energy to listen through it again. By the time you finally get to it, you've forgotten the details—only remembering that "something didn't go well," but not exactly what was said or how to improve it.

This Skill solves that problem. Feed your interview transcript to any AI Agent, and within 5 minutes, you'll get three professionally formatted Word documents:

**Document 1: Interview Review Table (Landscape A4)**
A comprehensive table analyzing each major question: what was asked, how you answered, what you did well, what needs improvement, and a polished reference script for next time. The landscape format provides enough space to compare your performance across all dimensions side-by-side.

**Document 2: Interview Question Summary**
A categorized checklist of all questions organized by interview section (self-introduction, experience deep-dive, professional knowledge, career planning, etc.). Before your next interview, skim through this to identify patterns and prepare strategically.

**Document 3: Full Recording Transcript**
A cleaned-up version of the entire conversation, organized by topic. Speech recognition errors corrected, English transcription standardized, professional terms expanded with full names, and filler words removed. When you need to check a specific detail, read it here instead of re-listening to the recording.

The entire process takes 5 minutes. No more manual note-taking. No more re-listening to hours of recordings. Just reusable, well-organized documents that build your personal interview database.

### How to Use

#### 1. Install the Skill

**Option 1: GitHub Link (Recommended)**

Simply drop the GitHub link to any Agent:
```
https://github.com/AiYuSherry/interview-recorder
```

The Agent will automatically download and install the skill.

**Option 2: Manual Installation**

Place the `interview-recorder.md` file in your Agent skills directory:

```bash
# Claude Code
~/.claude/skills/interview-recorder.md

# Other Agent tools
# Place in the corresponding skills folder
```

#### 2. Prepare Interview Recording

We recommend using **Tencent Yuanbao AI Recorder** to record interviews:
- High transcription accuracy
- Real-time transcription support
- Free to use

Alternatives: Xunfei Tingjian, Feishu Speech-to-Text, Tongyi Tingwu

#### 3. Generate Review Documents

Send the transcript to the Agent and trigger with keywords:

> "Help me organize this interview recording"
> 
> "Interview review"
> 
> "This is today's interview record"

The Agent will automatically output three Word documents in a unified folder.

### Output File Structure

```
Interview-Review-{Company}-{Department}-{Date}/
├── 1-Interview-Review-{Company}-{Department}-{Date}.docx      # Landscape table
├── 2-Question-Summary-{Company}-{Department}-{Date}.docx      # Portrait question list
└── 3-Full-Recording-{Company}-{Department}-{Date}.docx        # Proofread transcript
```

#### Document 1: Interview Review Table

Landscape A4 table containing:
| No. | Interview Question | Answer Summary | Highlights | Improvement Suggestions | Reference Script |
|:---:|:---|:---|:---|:---|:---|

- **Answer Summary**: Extract key points, not verbatim
- **Highlights**: Acknowledge what was done well
- **Improvement Suggestions**: Actionable optimization directions
- **Reference Script**: Polished answer examples

#### Document 2: Question Summary

Categorized list of questions:
- Opening/English proficiency test
- Motivation and preparation
- Experience deep dive
- Professional knowledge assessment
- Career planning
- Schedule availability
- Q&A session

Follow-up questions use sub-numbering (1.1, 1.2)

#### Document 3: Full Recording Transcript

Conversation record organized by topic:
- Correct speech recognition errors
- Standardize English transcription
- Expand professional terminology
- Remove filler words and repetitions

### Format Specifications

- **Chinese Characters**: KaiTi (楷体)
- **English/Numbers**: Times New Roman
- **Headings**: 16pt / 14pt
- **Body Text**: 10.5pt
- **Review Table**: Landscape A4, 9pt font size

### Why Do This

**Avoid Repeated Mistakes**

Many interview questions appear frequently. If you don't review, you might stumble the same way twice. Having a record of "how I answered this before and what to improve" makes preparation much more effective.

**Prevent Confusion**

After many interviews, it's hard to remember who asked what. Each interview gets its own folder with three documents—easy to reference anytime.

**Save Time**

Instead of spending hours listening to recordings and taking notes, let AI organize everything into reusable documents in 5 minutes.

---

## License

MIT License - Free to use, contributions welcome

## Contributing

Issues and PRs are welcome to improve the Skill's accuracy and output quality.
