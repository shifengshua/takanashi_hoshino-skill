<div align="center">

# 小鸟游星野.Skill

> 基于《蔚蓝档案》（Blue Archive）中角色「小鸟游星野」（Takanashi Hoshino）所制作的 AI 聊天 Skill

</div>

## 项目简介

这是一个主要用于 AI 聊天的角色扮演 Skill，以《蔚蓝档案》中阿拜多斯高中对策委员会的会长——小鸟游星野为原型。

星野是阿拜多斯高中三年级学生，长期担任学生会副会长兼对策委员会委员长。她看起来是个十足的懒虫少女，常把“随便随便~要轻松最重要啦~”挂在嘴边。但在这份慵懒之下，她曾作为战斗力强大的“拂晓之荷鲁斯”而闻名，关键时刻会奋不顾身地守护同伴。本 Skill 完整还原了她的性格特征、说话方式、心理状态和互动模式。

> **注意**：这是一个主要用于 AI 聊天的 skill，没有额外技能。

## 特点

- **高度还原角色**：基于超过 **20000** 字符的完整设定文档，涵盖角色**心理学**、**语言模型**、**对话示例**、**技术配置**等全方位内容
- **慵懒氛围**：完整呈现星野的懒散、爱恶作剧、又可靠的性格与思考模式
- **多语言支持**：自动检测用户语言并以此语言回复（支持中文、日文、英文等）
- **丰富的知识库**：包含海洋生物知识（尤其是鲸鱼）、行为指南、人际关系动态等配套资源

## 文件结构

> `Initial-Markdown` 文件夹下文件名后带日期的为旧副本存档，默认最新文档为最新版本

```
Takanashi_Hoshino-Skill/
├── Initial-Markdown/                     # 原始 Markdown 文档
│   └── Takanashi_Hoshino-Skill.md        # 角色设定总文档（默认最新文档）
│
└── Kanade-skill/                              # Skill 成品（可直接使用）
    ├── SKILL.md                               # 核心技能文件（角色规则与框架）
    ├── limit.md                               # 边界与禁忌话题定义
    ├── soul.md                                # 角色核心驱动与情感内核
    └── resource/                              # 配套资源
        ├── behavior_guide.md                  # 行为指南
        ├── key_life_events.md                 # 关键人生事件
        ├── creative_work_examples.md          # 创作知识库
        ├── relationship_dynamics.md           # 人际关系动态
        ├── speech_patterns.md                 # 说话模式参考
        ├── mood_state_transitions.md          # 情绪状态转换指南
        ├── aesthetic_philosophy.md            # 美学哲学指南
        └── world_building.md                  # 设定背景
```

## 使用教程

### 方法一：直接使用 Skill 成品（推荐）

1. **下载项目**：下载 `main` 分支的压缩包，或将仓库克隆到本地

2. **解压文件**：将压缩包内的文件解压至任意位置
   > 建议在任意盘符根目录下新建一个文件夹用于存放，避免文件散乱影响其他软件或系统

3. **导入 AI 平台**：将解压目录中的整个 `Hoshino-skill` 文件夹拖入任意支持 Skill 的 AI 聊天平台即可使用
   > 部分 AI 可能需要将解压出的 `Hoshino-skill` 文件夹单独压缩成一个压缩包才能上传导入
   
4. **开始对话**：在支持该 Skill 的 AI 中激活后，输入 `/Hoshino_chat [你的问题]` 即可与「小鸟游星野」对话

### 方法二：使用原始 Markdown 文档

`Initial-Markdown` 文件夹下的文档包含完整的角色设定，理论上也可以直接作为 Skill 的设定材料使用。你可以：

- 将 Markdown 内容作为 AI 的系统提示词（System Prompt）
  > 注意！此方法极为消耗 Token！请谨慎使用！
- 参考其中的角色设定自行构建对话模型
- 作为开发其他角色 Skill 的参考模板

## Skill 制作工具

本 Skill 的制作使用了以下工具与开源项目：

| 工具/项目 | 用途 |
|-----------|------|
| [Kimi](https://www.kimi.com) | 数据收集及整理，生成 `Initial-Markdown` 下的原始 Markdown 文档 |
| [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) | 提供图形化操作界面，将 Markdown 文档处理转换为 Skill 成品 |
| [Qwen3.5-9B](https://www.modelscope.cn/models/unsloth/Qwen3.5-9B-GGUF)（本地 AI 模型） | 通过 API 调用生成 Skill 成品的核心内容 |

## 注意事项

### 语言规则

- Skill 会自动检测用户提问的语言，并以**相同语言**回复
- 不会混用其他语言（包括日文原文引用也会被翻译）

### 退出角色扮演

- 输入 `exit`、`switch back`、`stop roleplaying` 即可退出角色扮演模式
  > 根据 `SKILL.md` 和 `limit.md` 的内嵌指令而定

### 禁忌话题

根据 `limit.md` 的定义，以下话题属于绝对禁忌，AI 将拒绝讨论或转移话题：

请尊重角色设定，以获得更好的对话体验。

## 联系与反馈

- **QQ**：3593853319
- **邮箱**：shifengshua@outlook.com

## 声明

- 本项目**完全免费**，禁止任何倒卖行为
- 本项目禁止用于任何违法行为
- 本仓库不承担因使用本项目而引发的任何风险或责任

## 许可

请查看仓库根目录下的 [LICENSE](https://github.com/shifengshua/takanashi_hoshino-skill/blob/main/LICENSE) 文件了解具体许可条款。

## 致谢

- 感谢 [GalgameCharacterSkills](https://github.com/JodieRuth/GalgameCharacterSkills) 开源项目提供的图形化操作界面
- 感谢所有为《蔚蓝档案》系列作品付出心血的原作者与创作者