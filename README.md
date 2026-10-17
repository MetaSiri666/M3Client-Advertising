# M3Client-Advertising

**English · [中文说明](#中文说明)**

M3Client-Advertising is a bilingual Codex skill for interviewing advertising clients and turning incomplete requests into a client Brief, three differentiated AI-video scripts, and three Hero Shots per concept.

It supports:

- TVC advertising films;
- AI digital humans;
- AI science and educational animation;
- AI government and enterprise promotional films;
- English and Chinese client conversations and deliverables;
- one-question-at-a-time interviews with numbered choices, multi-select, mixed ratios, custom answers, and skip/recommend options;
- optional client uploads, including logos, websites, company materials, product images, portraits, existing footage, and references;
- a client-safe output layer and a separate internal production-prompt package.

## Install

Place this repository at:

```text
~/.codex/skills/m3client-advertising
```

Then invoke it with:

```text
$m3client-advertising
```

The skill follows the language used by the client. To force English, begin in English or ask it to conduct the interview in English. To force Chinese, begin in Chinese or request a Chinese interview.

## Repository structure

```text
SKILL.md                  English runtime entry and language router
SKILL.zh-CN.md            Complete Chinese entry reference
agents/openai.yaml        Codex UI metadata
references/*.md           Chinese workflow references
references/en/*.md        Complete English workflow references
```

## Scope

This workflow is designed for an all-AI advertising company. It may use existing client footage and reference material, but it does not propose arranging new live-action filming. Internal generation prompts, model settings, negative prompts, and reference bindings are kept outside the client-facing conversation.

---

## 中文说明

M3Client-Advertising 是一套面向广告客户的双语 Codex Skill，用一问一答的方式把不完整需求整理成客户 Brief、三个差异化 AI 视频脚本，以及每案三张 Hero Shot。

支持：

- TVC 广告；
- AI 数字人；
- AI 动漫科普；
- AI 政企宣传片；
- 中英文客户访谈与交付；
- 每次只问一个问题，提供编号选项、多选、比例混合、自定义回答和跳过／建议；
- 客户自由上传 Logo、官网、公司资料、产品图、人物照片、已有视频和参考图；
- 客户可见交付层与内部生产提示词包分离。

### 安装

将整个仓库放到：

```text
~/.codex/skills/m3client-advertising
```

调用方式：

```text
$m3client-advertising
```

Skill 会自动跟随客户使用的语言。要使用英文访谈，以英文开始对话或明确要求英文；要使用中文访谈，以中文开始对话或明确要求中文。

### 仓库结构

```text
SKILL.md                  英文运行入口与语言路由
SKILL.zh-CN.md            完整中文入口参考
agents/openai.yaml        Codex 界面元数据
references/*.md           中文工作流参考文档
references/en/*.md        完整英文工作流参考文档
```

这是一套全 AI 广告制作流程，可以使用客户已有的实拍素材和参考资料，但不会建议安排新的真人、场地或产品实拍。生成提示词、模型参数、负面词和参考图绑定始终保留在内部制作层。
