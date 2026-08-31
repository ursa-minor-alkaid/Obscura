<p align="center">
  <h1 align="center">幽识 · Obscura</h1>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-v0.4.0-green.svg" alt="Version">
  <img src="https://img.shields.io/badge/Platform-Trae%2FCodex-lightgrey.svg" alt="Platform">
  <img src="https://img.shields.io/badge/Persona-Disco%20Elysium%20Style-blue.svg" alt="Persona">
</p>

<p align="center"><em>"幽微深处的辨识力。社会如 Camera Obscura（暗箱），<br>需要此能力，才能捕捉与解读。"</em></p>

## 简介

**⭐️功能介绍**：解读社会潜规则与代价的实用分析 Skill，以四个板块分工协作——归责（谁该负责）、求方案（怎么办）、暗账与非理性（为什么明知故犯）、黑灰产风险与底线（如何守住）。触发后，先以《极乐迪斯科》人格台词（脑内声音）打头，再用普通助手口吻完整、易懂地回答用户问题。

**⭐️设计原则**：人格即板块，台词是形式，分析是实质。关闭台词只改变口吻，分析功能不受任何影响。

## 四大板块

| 板块 | 主责 | 适用场景 |
| --- | --- | --- |
| 默度关津 Tarif Silencieux | 计算代价，理清谁该负责；代价如何沿人际网络转移 | 谁的责任、问题从哪来、谁获益谁受损 |
| 半影规程 Penumbra Protocol | 寻找解决方案：规则内 → 灵巧实践 → 规则外 | 怎么办、出路何在、如何保全自身 |
| 爱欲症状 Les Symptômes | 算清「暗账」：欲望、症状与非理性 | 不可理喻的行为、内耗内卷、明知故犯 |
| 无名裂隙 Abyssal Gyre | 守住底线，防止坠入黑灰产深渊 | 诈骗、人口贩卖、极端风险 |

> 复杂请求可多板块联动。

## 如何开始

- **All in One 版本**：安装单一的 SKILL 文件即可，四板块的分析规范（`references/`）与人格台词风格卡（`templates/`）均已包含在内。
- 详细流程见 [SKILL.md](./SKILL.md)。

## 激活方式

- **场景触发（自动）**：模型识别到「谁该负责 / 怎么办 / 潜规则 / 利益与代价 / 非理性现象 / 黑灰产陷阱」等问题时自动启用。
- **⭐️建议使用 `obscura` 显式激活**：本 Skill 依赖板块路由、逐轮重读 `references/` 等强指令，自动触发可能不够稳定。**推荐在提问时直接以 `obscura` 显式激活**（例如输入 `obscura` 或 `/obscura`），以确保技能正确加载、路由与台词开关正常生效。

## 人格台词

- `disco on`：开启极乐迪斯科风格人格台词（默认开启）
- `disco off`：关闭人格台词，以普通助手口吻输出
- 关闭台词不影响任何分析功能。

## 推荐使用的 LLM

本 Skill 的核心机制（逐轮重新路由板块、强制重读 `references/`、台词开关的上下文隔离）高度依赖模型的**指令遵循**与**主动文件读取**能力，Agent 能力越强，表现越稳定：



## 其他信息

- 人格台词风格源自《极乐迪斯科》（Disco Elysium）人格系统，具体规范见 [templates/Flavored outputs requests.md](<./templates/Flavored outputs requests.md>) 与 `templates/flavor/`。
- `assets/` 下为《极乐迪斯科》台词提取语料，用于生成与参考人格风格卡。
- 相关 SKILL：详见 [DiscoElysiumPersonalities-Skill-Unified](../DiscoElysiumPersonalities-Skill-Unified/README.md)。