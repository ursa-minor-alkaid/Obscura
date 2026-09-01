<p align="center">
  <img src="./assets/Obscura.jfif" width=150px>
  <h1 align="center">幽识 · Obscura</h1>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Persona-Disco%20Elysium%20Style-blue.svg" alt="Persona">
  <img src="https://img.shields.io/badge/version-v0.4.0-green.svg" alt="Version">
  <img src="https://img.shields.io/badge/Platform-Trae%2FCodex-lightgrey.svg" alt="Platform">
  </p>

<p align="center"><em>"Je voudrais être un agitateur pour les réguliers, et parvenir à ce qu'on laissât s'exprimer les irréguliers."<br>— Michel Foucault</em></p>

## 简介

**⭐️功能介绍**：解读社会规则与代价的实用分析 Skill。触发后，先以《极乐迪斯科》人格台词（脑内声音）开头，再用普通助手口吻完整、易懂地回答用户问题。

**⭐️设计目的**：结合自创的极乐迪人格，以一种较为有趣的方式为用户提供建议。

## 四大板块

| 板块 | 主责 | 适用场景 |
| --- | --- | --- |
| 默度关津 Tarif Silencieux | 计算代价，理清谁该负责；代价如何沿人际网络转移 | 谁的责任、问题从哪来、谁获益谁受损 |
| 半影规程 Penumbra Protocol | 寻找解决方案：规则内 → 灵巧实践 → 规则外 | 怎么办、出路何在、如何保全自身 |
| 爱欲症状 Les Symptômes | 算清「暗账」：欲望、症状与非理性 | 不可理喻的行为 |
| 无名裂隙 Abyssal Gyre | 守住底线，防止坠入黑灰产深渊 | 诈骗、人口贩卖、极端风险 |

> 复杂请求可多板块联动。

## 如何开始

**⭐️安装**：安装单一的 SKILL 文件即可，四板块的分析规范（`references/`）与人格台词风格卡（`templates/`）均已包含在内。

**⭐️激活方式：**

- **场景触发（自动）**：模型识别到「谁该负责 / 怎么办 / 潜规则 / 利益与代价 / 非理性现象 / 黑灰产陷阱」等问题时自动启用。
- **建议使用 `obscura` 显式激活**：本 Skill 依赖板块路由、逐轮重读 `references/` 等强指令，自动触发可能不够稳定。**推荐在提问时直接以 `obscura` 显式激活**（例如输入 `obscura` 或 `/obscura`），以确保技能正确加载、路由与台词开关正常生效。

**⭐️人格台词：**

- `disco on`：开启极乐迪斯科风格人格台词（默认开启）
- `disco off`：关闭人格台词，以普通助手口吻输出
- 关闭台词不影响任何分析功能。

## 推荐的 LLM

**⭐️注意事项：**

- 这个 skill 非常吃模型的 **agent 能力**和**文本处理能力**，需要使用两个方面都较强的模型才能得到较好的输出。
- 各家的模型使用自家的 Agent/Harness 软件效果会较好

**⭐️推荐模型名单：**

- Qwen 3.8-Max
- Kimi K3
- 其余尚未测试

**⭐️效果\*一般\*的模型：**

- DeepSeek v4 pro ga
- Seed 2.1 Pro/ Evolving
- 各家 Flash 模型（也许是世界知识太少了经常给抽象建议）

## 其他信息

- 相关 SKILL：详见 [DiscoElysiumPersonalities-Skill-Unified](../DiscoElysiumPersonalities-Skill-Unified/README.md)。
- 人格台词风格源自《极乐迪斯科》（Disco Elysium）人格系统，具体规范见 [templates/Flavored outputs requests.md](<./templates/Flavored outputs requests.md>) 与 `templates/flavor/`
- `assets/` 下为《极乐迪斯科》台词提取语料，用于生成与参考人格风格卡。
