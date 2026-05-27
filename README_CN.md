# Awesome Anti AI Slop

> 精选用于减少 **AI 味 / AI slop** 的开源项目、skills、prompts、CLI、GitHub Actions 与工作流。  
> 目标是让文本、代码、PR、UI 和产品输出更自然、更具体、更有审美、更可维护，而不是追求“绕过检测器”。

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Last Updated](https://img.shields.io/badge/updated-2026--05--27-blue)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)

## What is AI slop?

这里的 **AI slop** 指由 AI 生成或辅助生成时常见的低质量痕迹，例如：

- 空洞、模板化、过度平滑的文字；
- “不仅……而且……”“总之”“值得注意的是”等机械连接词；
- 大量正确但没洞察的泛泛而谈；
- 代码里看似完整但缺少边界条件、测试、异常处理；
- PR 里批量生成的低质量改动；
- UI 里千篇一律的卡片、渐变、居中 hero、无意义动效；
- 设计语言、排版、间距、信息层级缺乏判断力。

这个列表关注 **质量提升、风格校准、审美增强、工程治理**，不收录纯粹宣传“undetectable / bypass detector”的低质量项目。

## Selection Criteria

优先收录：

1. **开源且可直接使用**：Skill、Prompt、CLI、App、GitHub Action、linter、规则集。
2. **真实解决 AI slop**：能改善文字、代码、PR、UI、设计或工作流质量。
3. **有关注度或独特价值**：star / fork / 使用场景 / 实现质量至少有一项突出。
4. **不是简单营销壳**：避免只包装第三方 API、只宣传绕过检测器、无实际规则或源码的项目。
5. **可组合进工作流**：能放进 Claude Code、Codex、Cursor、ChatGPT、CI、pre-commit 或团队规范。

> Star badge 是动态的，排序主要参考初次整理时的关注度与实用性。GitHub stars 会随时间变化。

## Contents

- [Best Picks](#best-picks)
- [Starter Stacks](#starter-stacks)
- [Text & Writing](#text--writing)
- [Chinese Writing](#chinese-writing)
- [Academic Writing](#academic-writing)
- [Frontend, UI & Design Taste](#frontend-ui--design-taste)
- [Code, PR & Engineering Slop](#code-pr--engineering-slop)
- [Apps, CLIs & Workbenches](#apps-clis--workbenches)
- [Directories & Meta Lists](#directories--meta-lists)
- [Niche / Experimental](#niche--experimental)
- [How to Evaluate an Anti-Slop Tool](#how-to-evaluate-an-anti-slop-tool)
- [Contributing](#contributing)
- [License](#license)

## Best Picks

| Project | Stars | Best for | Why it matters |
|---|---:|---|---|
| [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | [![Stars](https://img.shields.io/github/stars/pbakaus/impeccable?style=social)](https://github.com/pbakaus/impeccable) | Frontend / UI / design anti-slop | 高关注度前端与设计反 AI 味工具，适合解决 AI 生成网页的模板感、廉价感和视觉同质化。 |
| [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | [![Stars](https://img.shields.io/github/stars/Leonxlnx/taste-skill?style=social)](https://github.com/Leonxlnx/taste-skill) | AI-built frontend taste | Anti-slop frontend framework for AI agents，强调 layout、typography、motion、spacing、design taste，可用于 Codex、Cursor、Claude Code 等。 |
| [blader/humanizer](https://github.com/blader/humanizer) | [![Stars](https://img.shields.io/github/stars/blader/humanizer?style=social)](https://github.com/blader/humanizer) | English writing humanizer | 英文通用文本去 AI 味代表项目，适合文章、文档、邮件、产品文案。 |
| [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | [![Stars](https://img.shields.io/github/stars/Imbad0202/academic-research-skills?style=social)](https://github.com/Imbad0202/academic-research-skills) | Research / academic workflow | 学术研究与写作综合 skill 集，不是单纯 humanizer，而是研究质量与写作质量工具箱。 |
| [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | [![Stars](https://img.shields.io/github/stars/op7418/Humanizer-zh?style=social)](https://github.com/op7418/Humanizer-zh) | 中文写作 | 中文去 AI 味首选之一，适合中文文章、中文学术初稿、公众号、商业文案。 |
| [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) | [![Stars](https://img.shields.io/github/stars/hardikpandya/stop-slop?style=social)](https://github.com/hardikpandya/stop-slop) | Prompt rules / prose cleanup | 规则型 anti-slop skill，适合作为自定义指令、system prompt、Claude Project 规则底稿。 |
| [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | [![Stars](https://img.shields.io/github/stars/conorbronsdon/avoid-ai-writing?style=social)](https://github.com/conorbronsdon/avoid-ai-writing) | Detect + rewrite workflow | 支持发现 AI 写作痕迹并重写，适合内容团队、博客、产品文档。 |
| [peakoss/anti-slop](https://github.com/peakoss/anti-slop) | [![Stars](https://img.shields.io/github/stars/peakoss/anti-slop?style=social)](https://github.com/peakoss/anti-slop) | GitHub PR quality gate | 用 GitHub Action 识别低质量或 AI slop PR，适合开源项目与团队仓库治理。 |
| [mshumer/unslop](https://github.com/mshumer/unslop) | [![Stars](https://img.shields.io/github/stars/mshumer/unslop?style=social)](https://github.com/mshumer/unslop) | Custom anti-slop instructions | 从样本中发现模型默认套路并生成定制 instruction file，适合品牌、团队、产品风格校准。 |
| [brandonwise/humanizer](https://github.com/brandonwise/humanizer) | [![Stars](https://img.shields.io/github/stars/brandonwise/humanizer?style=social)](https://github.com/brandonwise/humanizer) | CLI / local audit | 低星但实用，包含评分、分析、报告、建议、扫描、对比等本地工作流。 |

## Starter Stacks

### 中文写作

- [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) — 主力中文去 AI 味。
- [cangtianhuang/humanizer-academic-zh](https://github.com/cangtianhuang/humanizer-academic-zh) — 中文学术写作专用。
- [marswjf/stop-slop-zh](https://github.com/marswjf/stop-slop-zh) — 中英双语规则型 de-slop skill。
- [1-SKILL/shuorenhua](https://github.com/1-SKILL/shuorenhua) — 中文“说人话”方向的小型项目。

### 英文博客 / 文档 / 产品文案

- [blader/humanizer](https://github.com/blader/humanizer) — 主力 humanizer。
- [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) — 规则底稿。
- [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) — detect + rewrite。
- [jalaalrd/anti-ai-slop-writing](https://github.com/jalaalrd/anti-ai-slop-writing) — 轻量 anti-slop writing prompt。

### 前端 / UI / 产品设计

- [pbakaus/impeccable](https://github.com/pbakaus/impeccable) — 前端/UI anti-slop。
- [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) — AI-built frontend taste framework。
- [mshumer/unslop](https://github.com/mshumer/unslop) — 生成团队专属反 slop 指令。
- [Wholiver/swiftui-design-skill](https://github.com/Wholiver/swiftui-design-skill) — SwiftUI 设计方向。
- [Hacksore/oghunt](https://github.com/Hacksore/oghunt) — Product Hunt 信息流去 AI 噪声。

### 代码 / PR / 团队治理

- [peakoss/anti-slop](https://github.com/peakoss/anti-slop) — GitHub Action。
- [scanaislop/aislop](https://github.com/scanaislop/aislop) — AI code quality gate / hook / MCP。
- [JordanGunn/agent-slop-lint](https://github.com/JordanGunn/agent-slop-lint) — agentic coding linter。
- [yuvrajangadsingh/vibecheck](https://github.com/yuvrajangadsingh/vibecheck) — JS/TS/Python slop lint。
- [HugoLopes45/llmstrip](https://github.com/HugoLopes45/llmstrip) — 轻量清理 prose / comments / commits。

## Text & Writing

| Project | Stars | Type | Notes |
|---|---:|---|---|
| [blader/humanizer](https://github.com/blader/humanizer) | [![Stars](https://img.shields.io/github/stars/blader/humanizer?style=social)](https://github.com/blader/humanizer) | Skill | 英文通用写作、文档、博客、邮件去 AI 味。 |
| [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) | [![Stars](https://img.shields.io/github/stars/hardikpandya/stop-slop?style=social)](https://github.com/hardikpandya/stop-slop) | Skill / rules | 识别 banned phrases、结构套路、句子级 AI 痕迹。 |
| [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | [![Stars](https://img.shields.io/github/stars/conorbronsdon/avoid-ai-writing?style=social)](https://github.com/conorbronsdon/avoid-ai-writing) | Skill / workflow | Detect 与 Rewrite 两种模式，适合内容团队。 |
| [jalaalrd/anti-ai-slop-writing](https://github.com/jalaalrd/anti-ai-slop-writing) | [![Stars](https://img.shields.io/github/stars/jalaalrd/anti-ai-slop-writing?style=social)](https://github.com/jalaalrd/anti-ai-slop-writing) | Prompt | 针对词汇、结构、标点、格式的轻量规则包。 |
| [coderjatin/anti-slop-writing](https://github.com/coderjatin/anti-slop-writing) | [![Stars](https://img.shields.io/github/stars/coderjatin/anti-slop-writing?style=social)](https://github.com/coderjatin/anti-slop-writing) | Prompt | 可用于 Claude Code、Gemini CLI、Codex CLI、Copilot、Cursor 等。 |
| [stephenturner/skill-deslop](https://github.com/stephenturner/skill-deslop) | [![Stars](https://img.shields.io/github/stars/stephenturner/skill-deslop?style=social)](https://github.com/stephenturner/skill-deslop) | Skill | 科学/技术写作 de-slop，针对公式化结构、filler、false agency。 |
| [rankgnar/deslop](https://github.com/rankgnar/deslop) | [![Stars](https://img.shields.io/github/stars/rankgnar/deslop?style=social)](https://github.com/rankgnar/deslop) | CLI | 检测/移除 buzzwords、false profundity、空洞转折。 |
| [AUAggy/deslop](https://github.com/AUAggy/deslop) | [![Stars](https://img.shields.io/github/stars/AUAggy/deslop?style=social)](https://github.com/AUAggy/deslop) | VS Code / rewrite | 选择文本后按严格规则重写，不生成新内容。 |
| [gabelul/slopbuster](https://github.com/gabelul/slopbuster) | [![Stars](https://img.shields.io/github/stars/gabelul/slopbuster?style=social)](https://github.com/gabelul/slopbuster) | Audit / rules | prose、code、academic writing 审查，包含多模式 audit 思路。 |
| [ksanyok/TextHumanize](https://github.com/ksanyok/TextHumanize) | [![Stars](https://img.shields.io/github/stars/ksanyok/TextHumanize?style=social)](https://github.com/ksanyok/TextHumanize) | Library | 离线算法库，多语言文本归一化；不应被当作检测器绕过保证。 |
| [HugoLopes45/llmstrip](https://github.com/HugoLopes45/llmstrip) | [![Stars](https://img.shields.io/github/stars/HugoLopes45/llmstrip?style=social)](https://github.com/HugoLopes45/llmstrip) | Rust CLI | 处理 prose、代码注释、commit 信息里的 LLM 痕迹。 |
| [avectats7/anti-ai-writing](https://github.com/avectats7/anti-ai-writing) | [![Stars](https://img.shields.io/github/stars/avectats7/anti-ai-writing?style=social)](https://github.com/avectats7/anti-ai-writing) | Prompt | 英语/西语规则包，针对 banned words、phrases、structures。 |

## Chinese Writing

| Project | Stars | Type | Notes |
|---|---:|---|---|
| [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | [![Stars](https://img.shields.io/github/stars/op7418/Humanizer-zh?style=social)](https://github.com/op7418/Humanizer-zh) | Skill | 中文去 AI 味主力项目，适合中文稿件、商业文案、中文论文初稿。 |
| [cangtianhuang/humanizer-academic-zh](https://github.com/cangtianhuang/humanizer-academic-zh) | [![Stars](https://img.shields.io/github/stars/cangtianhuang/humanizer-academic-zh?style=social)](https://github.com/cangtianhuang/humanizer-academic-zh) | Prompt / skill | 中文学术写作去 AI 痕迹。 |
| [marswjf/stop-slop-zh](https://github.com/marswjf/stop-slop-zh) | [![Stars](https://img.shields.io/github/stars/marswjf/stop-slop-zh?style=social)](https://github.com/marswjf/stop-slop-zh) | Skill / prompt | 中英双语 de-slop skill，可用于 Claude Code、OpenClaw、Codex CLI、Cursor/Windsurf 等。 |
| [shyuan/writing-humanizer](https://github.com/shyuan/writing-humanizer) | [![Stars](https://img.shields.io/github/stars/shyuan/writing-humanizer?style=social)](https://github.com/shyuan/writing-humanizer) | Plugin / skill | 台湾繁中写作 humanizer。 |
| [1-SKILL/shuorenhua](https://github.com/1-SKILL/shuorenhua) | [![Stars](https://img.shields.io/github/stars/1-SKILL/shuorenhua?style=social)](https://github.com/1-SKILL/shuorenhua) | Skill | 中文“说人话”改写，小众但方向明确。 |

## Academic Writing

| Project | Stars | Type | Notes |
|---|---:|---|---|
| [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | [![Stars](https://img.shields.io/github/stars/Imbad0202/academic-research-skills?style=social)](https://github.com/Imbad0202/academic-research-skills) | Skill collection | 学术研究、论文写作、质量检查、风格校准的综合技能集。 |
| [cangtianhuang/humanizer-academic-zh](https://github.com/cangtianhuang/humanizer-academic-zh) | [![Stars](https://img.shields.io/github/stars/cangtianhuang/humanizer-academic-zh?style=social)](https://github.com/cangtianhuang/humanizer-academic-zh) | Chinese academic | 中文学术写作专用 anti-AI-trace prompt/skill。 |
| [stephenturner/skill-deslop](https://github.com/stephenturner/skill-deslop) | [![Stars](https://img.shields.io/github/stars/stephenturner/skill-deslop?style=social)](https://github.com/stephenturner/skill-deslop) | Scientific / technical | 科学写作、技术博客、研究沟通中的 de-slop。 |
| [gabelul/slopbuster](https://github.com/gabelul/slopbuster) | [![Stars](https://img.shields.io/github/stars/gabelul/slopbuster?style=social)](https://github.com/gabelul/slopbuster) | Audit | prose/code/academic writing 审查与评分思路。 |

## Frontend, UI & Design Taste

| Project | Stars | Type | Notes |
|---|---:|---|---|
| [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | [![Stars](https://img.shields.io/github/stars/pbakaus/impeccable?style=social)](https://github.com/pbakaus/impeccable) | Frontend / UI skill | 前端/UI/design anti-slop 第一梯队，适合纠正 AI 生成网页的模板感。 |
| [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | [![Stars](https://img.shields.io/github/stars/Leonxlnx/taste-skill?style=social)](https://github.com/Leonxlnx/taste-skill) | Frontend skill framework | Gives your AI good taste. 强调 layout、typography、motion、spacing、design-system、redesign audit 与 image-to-code 流程。 |
| [mshumer/unslop](https://github.com/mshumer/unslop) | [![Stars](https://img.shields.io/github/stars/mshumer/unslop?style=social)](https://github.com/mshumer/unslop) | Instruction generator | 从文本或视觉样本中发现模型默认套路，生成可复用 instruction file。 |
| [Wholiver/swiftui-design-skill](https://github.com/Wholiver/swiftui-design-skill) | [![Stars](https://img.shields.io/github/stars/Wholiver/swiftui-design-skill?style=social)](https://github.com/Wholiver/swiftui-design-skill) | SwiftUI design skill | SwiftUI 设计方向，适合移动端 UI 质量提升。 |
| [Hacksore/oghunt](https://github.com/Hacksore/oghunt) | [![Stars](https://img.shields.io/github/stars/Hacksore/oghunt?style=social)](https://github.com/Hacksore/oghunt) | Product Hunt filter | 从 Product Hunt 信息流中移除 AI listing，偏信息噪声治理。 |

### Taste Skill install example

```bash
npx skills add https://github.com/Leonxlnx/taste-skill
npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"
```

Use it when the problem is not “this text sounds AI-generated”, but “this interface looks AI-generated”.

## Code, PR & Engineering Slop

| Project | Stars | Type | Notes |
|---|---:|---|---|
| [peakoss/anti-slop](https://github.com/peakoss/anti-slop) | [![Stars](https://img.shields.io/github/stars/peakoss/anti-slop?style=social)](https://github.com/peakoss/anti-slop) | GitHub Action | 检测并关闭低质量或 AI slop PR。 |
| [JordanGunn/agent-slop-lint](https://github.com/JordanGunn/agent-slop-lint) | [![Stars](https://img.shields.io/github/stars/JordanGunn/agent-slop-lint?style=social)](https://github.com/JordanGunn/agent-slop-lint) | Linter | 面向 agentic coding 的语言无关代码质量 linter。 |
| [scanaislop/aislop](https://github.com/scanaislop/aislop) | [![Stars](https://img.shields.io/github/stars/scanaislop/aislop?style=social)](https://github.com/scanaislop/aislop) | Hook / MCP / quality gate | 面向 Claude Code、Cursor、Codex 的 AI 代码质量门禁。 |
| [yuvrajangadsingh/vibecheck](https://github.com/yuvrajangadsingh/vibecheck) | [![Stars](https://img.shields.io/github/stars/yuvrajangadsingh/vibecheck?style=social)](https://github.com/yuvrajangadsingh/vibecheck) | JS/TS/Python linter | 类似 ESLint 的 AI slop 检测。 |
| [adamcharnock/deslop](https://github.com/adamcharnock/deslop) | [![Stars](https://img.shields.io/github/stars/adamcharnock/deslop?style=social)](https://github.com/adamcharnock/deslop) | pre-commit prose lint | 提交前检查文档和 prose 中的 AI 写作模式。 |
| [HugoLopes45/llmstrip](https://github.com/HugoLopes45/llmstrip) | [![Stars](https://img.shields.io/github/stars/HugoLopes45/llmstrip?style=social)](https://github.com/HugoLopes45/llmstrip) | CLI | 清理代码注释、commit message、prose 中的 LLM 痕迹。 |

## Apps, CLIs & Workbenches

| Project | Stars | Type | Notes |
|---|---:|---|---|
| [lynote-ai/humanize-text](https://github.com/lynote-ai/humanize-text) | [![Stars](https://img.shields.io/github/stars/lynote-ai/humanize-text?style=social)](https://github.com/lynote-ai/humanize-text) | App | App 型 AI text humanizer，关注度较高；建议只作为自然化编辑器使用。 |
| [DadaNanjesha/AI-Text-Humanizer-App](https://github.com/DadaNanjesha/AI-Text-Humanizer-App) | [![Stars](https://img.shields.io/github/stars/DadaNanjesha/AI-Text-Humanizer-App?style=social)](https://github.com/DadaNanjesha/AI-Text-Humanizer-App) | App | 正式、人类化、学术风格改写 App。 |
| [brandonwise/humanizer](https://github.com/brandonwise/humanizer) | [![Stars](https://img.shields.io/github/stars/brandonwise/humanizer?style=social)](https://github.com/brandonwise/humanizer) | CLI / OpenClaw skill | 本地评分、分析、报告、建议、扫描、对比等功能较完整。 |
| [rudra496/StealthHumanizer](https://github.com/rudra496/StealthHumanizer) | [![Stars](https://img.shields.io/github/stars/rudra496/StealthHumanizer?style=social)](https://github.com/rudra496/StealthHumanizer) | App / multi-provider | 多 provider、多重写等级；“stealth/bypass”倾向明显，谨慎使用。 |
| [ZAYUVALYA/AI-Text-Humanizer](https://github.com/ZAYUVALYA/AI-Text-Humanizer) | [![Stars](https://img.shields.io/github/stars/ZAYUVALYA/AI-Text-Humanizer?style=social)](https://github.com/ZAYUVALYA/AI-Text-Humanizer) | App / paraphrasing | 上下文感知 paraphrasing，早期阶段。 |
| [dixon2004/ai-humanizer](https://github.com/dixon2004/ai-humanizer) | [![Stars](https://img.shields.io/github/stars/dixon2004/ai-humanizer?style=social)](https://github.com/dixon2004/ai-humanizer) | Web/local app | Gemini 驱动的小型 humanizer。 |
| [puneethkotha/humanizer-workbench](https://github.com/puneethkotha/humanizer-workbench) | [![Stars](https://img.shields.io/github/stars/puneethkotha/humanizer-workbench?style=social)](https://github.com/puneethkotha/humanizer-workbench) | CLI / skill | humanizer workbench，小众项目。 |
| [itsjwill/humanizer-x](https://github.com/itsjwill/humanizer-x) | [![Stars](https://img.shields.io/github/stars/itsjwill/humanizer-x?style=social)](https://github.com/itsjwill/humanizer-x) | Agent / workflow | 4-pass humanizer + voice agent，小众项目。 |

## Directories & Meta Lists

| Project / Topic | Stars | Notes |
|---|---:|---|
| [shannhk/avoid-slop](https://github.com/shannhk/avoid-slop) | [![Stars](https://img.shields.io/github/stars/shannhk/avoid-slop?style=social)](https://github.com/shannhk/avoid-slop) | 专门收集 text、code、design 反 AI slop 工具。 |
| [GitHub Topic: ai-humanizer](https://github.com/topics/ai-humanizer) | - | 文本 humanizer app / skill / prompt 集合。 |
| [GitHub Topic: humanize-text](https://github.com/topics/humanize-text) | - | 更窄的文本 humanizer topic。 |
| [GitHub Topic: ai-slop](https://github.com/topics/ai-slop) | - | 覆盖 PR、代码、UI、设计、内容噪声等更广义 AI slop。 |

## Niche / Experimental

这些项目关注度较低、场景较窄，或宣传口径里包含较多“undetectable / bypass”倾向。可以参考实现与规则，不建议无脑依赖。

| Project | Stars | Notes |
|---|---:|---|
| [Aboudjem/humanizer-skill](https://github.com/Aboudjem/humanizer-skill) | [![Stars](https://img.shields.io/github/stars/Aboudjem/humanizer-skill?style=social)](https://github.com/Aboudjem/humanizer-skill) | Claude Code skill，包含多模式与 voice profile。 |
| [Firdavs-coder/ai_humanizer](https://github.com/Firdavs-coder/ai_humanizer) | [![Stars](https://img.shields.io/github/stars/Firdavs-coder/ai_humanizer?style=social)](https://github.com/Firdavs-coder/ai_humanizer) | 更偏 prompt/model release。 |
| [Hakku/finnish-humanizer](https://github.com/Hakku/finnish-humanizer) | [![Stars](https://img.shields.io/github/stars/Hakku/finnish-humanizer?style=social)](https://github.com/Hakku/finnish-humanizer) | 芬兰语 humanizer。 |
| [lguz/humanize-writing-skill](https://github.com/lguz/humanize-writing-skill) | [![Stars](https://img.shields.io/github/stars/lguz/humanize-writing-skill?style=social)](https://github.com/lguz/humanize-writing-skill) | Claude skill，三段式编辑思路。 |
| [199-biotechnologies/humanise-text-skill](https://github.com/199-biotechnologies/humanise-text-skill) | [![Stars](https://img.shields.io/github/stars/199-biotechnologies/humanise-text-skill?style=social)](https://github.com/199-biotechnologies/humanise-text-skill) | Claude Code skill，规则清单型。 |
| [diaiq/claude-skill-humanizer](https://github.com/diaiq/claude-skill-humanizer) | [![Stars](https://img.shields.io/github/stars/diaiq/claude-skill-humanizer?style=social)](https://github.com/diaiq/claude-skill-humanizer) | Claude Code skill，注意甄别检测器绕过宣传。 |
| [imsv1301/unmask-ai](https://github.com/imsv1301/unmask-ai) | [![Stars](https://img.shields.io/github/stars/imsv1301/unmask-ai?style=social)](https://github.com/imsv1301/unmask-ai) | 检测 + humanize 包装。 |
| [ofershap/ai-humanizer](https://github.com/ofershap/ai-humanizer) | [![Stars](https://img.shields.io/github/stars/ofershap/ai-humanizer?style=social)](https://github.com/ofershap/ai-humanizer) | 低星项目，宣传偏 undetectable，谨慎。 |
| [asazonov/deslop-codex](https://github.com/asazonov/deslop-codex) | [![Stars](https://img.shields.io/github/stars/asazonov/deslop-codex?style=social)](https://github.com/asazonov/deslop-codex) | Codex skill package，关注度较低。 |

## How to Evaluate an Anti-Slop Tool

使用任何 anti-slop / humanizer 工具前，建议检查：

1. **是否只是在同义词替换**  
   低质量 humanizer 常常只是替换词、插入口语、增加错别字。真正有用的工具应该能改善结构、信息密度、细节、节奏、语气与上下文一致性。

2. **是否承诺绕过检测器**  
   AI 检测器本身误判率高，且会不断变化。过度宣传“bypass Turnitin / GPTZero”的项目通常不值得信任。

3. **是否保留事实与意图**  
   好的改写不应凭空增加事实、不应改变观点、不应删除关键限制条件。

4. **是否支持你的工作流**  
   最好能作为 skill、CLI、pre-commit、GitHub Action、IDE 插件或团队 prompt 直接接入。

5. **是否有可维护规则**  
   规则集越透明，越容易被团队调整。黑盒 API 包装器通常不利于长期使用。

6. **是否能处理你的语言与场景**  
   中文、英文、学术、前端 UI、代码 PR、品牌文案的 slop 痕迹并不相同，尽量选择场景匹配的项目。

## Suggested Workflow

### For writing

1. 先让模型写出信息完整的初稿。
2. 用 anti-slop 规则检查结构、措辞、节奏、空话。
3. 手动补充个人经验、具体数据、案例、限制条件。
4. 再用 humanizer 做局部润色，而不是整篇无脑改写。
5. 最后做事实核查和风格统一。

### For frontend

1. 先定义产品气质、受众、信息层级，而不是直接让 AI “make it beautiful”。
2. 用 [taste-skill](https://github.com/Leonxlnx/taste-skill) 或 [impeccable](https://github.com/pbakaus/impeccable) 约束布局、排版、动效、间距。
3. 对 AI 生成 UI 做 redesign audit。
4. 删除模板 hero、廉价渐变、无意义卡片、重复 CTA。
5. 以真实内容和真实状态测试界面，而不是只看空壳 mockup。

### For code and PRs

1. 为 AI 生成代码设置明确的边界条件、测试要求和验收标准。
2. 用 linter / GitHub Action 阻止低质量批量 PR。
3. 要求每个 PR 解释意图、风险、测试方式，而不是只提交“refactor”。
4. 对 AI 改动做 diff review，不接受无意义重排、注释膨胀、假抽象。
5. 把常见失败模式写进团队 agent rules。

## Contributing

欢迎提交 PR。建议每个新增项目包含：

```markdown
- [owner/repo](https://github.com/owner/repo) - 一句话说明用途。
  - Type: Skill / Prompt / CLI / App / GitHub Action / Linter / Directory
  - Best for: 中文写作 / 英文文档 / 学术 / 前端 / PR / 代码质量 / 设计
  - Why it matters: 它解决什么 AI slop 问题？
  - Caveat: 是否有检测器绕过宣传、是否维护不活跃、是否依赖闭源 API？
```

不建议收录：

- 只宣传 “100% undetectable” 的项目；
- 无源码、无规则、无文档的壳项目；
- 重复 fork 且没有新增价值的项目；
- 纯闭源 SaaS；
- 鼓励学术不诚信或规避检测责任的工具。

## License

建议使用 [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/) 或 MIT 发布这个列表。正式开源前请在仓库中加入你选择的 LICENSE 文件。
