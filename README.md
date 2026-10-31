# reduce-ai

两个写作 skill：`reduce-ai-zh`（中文）和 `reduce-ai-en`（英文）。在 AI 辅助写作论文、学位论文、README、技术文档等成段文本时加载，让输出读起来自然、克制、像行内人写的，而不是一股模板机器腔。

它们是生成时约束，不是事后润色器：规则在动笔前加载，一次写完，没有"先生成再改写"的第二遍。

## 它治什么病

AI 辅助写作的通病在结构，不在个别词。典型症状：

- 每段结尾替读者总结："这充分说明……的重要性""This underscores the critical role of..."
- 机械总分总：首先/其次/最后，段段有小结，章章有排比式小结
- 膨胀形容堆在空洞处："显著提升""广阔前景"，没有一个具体数字
- 四字连排、rule of three、修饰性连接词成串

核心规则共十二条，分硬约束（事实零改动、引用原样保留、术语一致）、结构原则（具体优先、不点题说教、段落句长自然起伏、连接词服务逻辑）、语言习惯（朴素动词、限定词对应真实确定性）。另有词表作参考——用法是规避，不是替换；替代说法反复使用自己就会变成新的机器腔。

规则刻意的少。规则越多，执行越用力，刻意感越重，而刻意感本身就是机器腔。

## 安装

一条命令（支持 Claude Code、Cursor、ZCode 等 50+ 工具，自动检测）：

```bash
# 从 GitHub
npx skills add https://github.com/petra1218/reduce-ai

# 或从 GitCode（国内访问更快）
npx skills add https://gitcode.com/petra1218/reduce-ai
```

只要其中一个语言版本时加 `--skill reduce-ai-zh` 或 `--skill reduce-ai-en`。

手动安装：把 `skills/` 下对应目录复制到 `~/.agents/skills/`（全局）或项目的 `.agents/skills/`。

## 使用

安装后正常使用即可。写中文成段文本时 `reduce-ai-zh` 会自动触发；也可以显式要求"用 reduce-ai-zh 写这段绪论"。英文同理。

每个 skill 附带两类可插拔配置，写作前按需读取：

```
skills/reduce-ai-zh/
├── SKILL.md                        # 十二条核心规则（始终生效）
└── references/
    ├── genres/
    │   ├── thesis.md               # 学位论文：摘要/绪论/综述/结论的写法
    │   └── readme-docs.md          # README/发布说明/使用文档
    ├── disciplines/
    │   └── engineering-management.md   # 工程管理（行业惯用语 vs 膨胀话的区分）
    └── vocabulary.md               # 机器腔词表（参考用，非替换表）
```

英文版同构。学科和文体库按需扩充，见下方"参与"。

## 边界说明

这个项目解决文风问题，不以通过 AI 检测器为目标，也不对任何检测结果负责。AI 检测工具本身不可靠（对非母语作者的误报率尤其高），把"过检测"当目标会把文本改坏，而且无法兑现。如果你的机构有 AI 使用披露政策，遵守它。

## 参与

三层贡献入口，成本从低到高：

1. 往 `vocabulary.md` 加词，PR 附上下文说明
2. 照模板写一个学科 profile（一个文件：行业惯用语、本学科膨胀话、真实感来源、方法写作清单）
3. 写一个新文体 profile

模板和自检要求见 [CONTRIBUTING.md](CONTRIBUTING.md)。目前内置工程管理一个学科和学位论文、开源文档两个文体，其余等你的 PR。

## 致谢

核心规则的提炼参考了这些公开工作：Wikipedia 的 [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) 指南，[humanizer_academic](https://github.com/matsuikentaro1/humanizer_academic)（35 模式库及其"保留逻辑连接词"的修正经验），[unslop](https://github.com/asavvin-pixel/unslop)（结构信号优先于词汇信号的三层方法），[Humanizer-zh](https://github.com/op7418/Humanizer-zh)（中文去机器腔的编辑原则），以及 Matsui (2025)、Geng & Trotta (ACL 2025) 对学术写作词汇漂移的实证研究。

## 许可

[MIT](LICENSE)

---

reduce-ai ships two skills — `reduce-ai-zh` and `reduce-ai-en` — generation-time writing constraints that keep AI-assisted theses, papers, and project docs reading natural and restrained, in Chinese and English. Install with `npx skills add https://github.com/petra1218/reduce-ai`. MIT.
