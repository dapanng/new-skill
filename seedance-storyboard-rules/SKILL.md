---
name: "seedance-storyboard-rules"
description: "Seedance 2.0 微短剧分镜全局规则体系，涵盖规定情境分析、情绪浓度值体系、视觉渲染、镜头拆分、空间连续性、景别衔接、运镜、表演、潜台词、群像、声音设计、台词处理、肢体动作、分镜三层级、提示词优化等 25 项规则。Invoke when 用户进行微短剧分镜创作、镜头拆分、Seedance 2.0 提示词编写、电影级 CG 分镜设计，或需要套用固定分镜模板时。"
---

# Seedance 2.0 微短剧分镜全局规则

## 概述

本 Skill 定义了使用 Seedance 2.0 进行微短剧分镜创作的全套全局规则，共 25 节，覆盖规定情境分析、核心分析公理、情绪浓度值体系、视觉渲染、镜头拆分、空间连续性、景别衔接、运镜、表演、潜台词、群像、声音设计、台词处理、肢体动作、分镜设计三层级、提示词优化等全链路要素。

**核心理念**：

- 空间先成立，动作再发生。
- 人物先有关系，镜头再有情绪。
- 上一镜必须给下一镜留下站位和视线依据。
- 一个视频只解决一个主要动作或情绪问题。
- 人物情绪用微动作表现，不靠夸张表情。
- 物件必须参与叙事，不做无意义展示。
- 群像负责制造社会压力，主角负责制造戏剧核心。
- 镜头不追求复杂，追求因果关系。

**最终形成的因果链路**：

```
空间建立 → 动作触发 → 人物反应 → 情绪变化 → 台词落点 → 下一镜承接
```

---

## 加载时必读

按以下顺序阅读本 Skill 的各主题文件：

1. **`visual-rendering.md`** — 一、全局视觉渲染规则（风格非固定、7 种风格可选、通用质量基底、按风格调整皮肤质感、禁止项）。
2. **`shot-splitting.md`** — 二、Seedance 2.0 单个视频的镜头拆分原则（一视频一动作、A/B/C/D 镜拆分法、时长建议）。
3. **`shot-composition.md`** — 三、画面运作规则（焦点角色分类、单一视觉核心原则）。
4. **`spatial-continuity.md`** — 四、人物站位与物理空间连续性（空间锁定、连续性规则、空间锚点）。
5. **`shot-transitions.md`** — 五、电影级景别衔接规则（景别递进链路、衔接技法）。
6. **`camera-movement.md`** — 六、镜头运动规则（慢推、环绕、手持、静止、焦点转移、插入镜头）。
7. **`acting.md`** — 七、人物表演规则（禁止单一情绪词、微动作清单、表情三段式）。
8. **`subtext.md`** — 八、人物潜台词规则（嘴上说什么 vs 心里想什么）。
9. **`dual-layer-acting.md`** — 九、双层人物表演规则（外层 vs 内层、表情在演眼睛泄密）。
10. **`ensemble.md`** — 十、群像规则（群演反应多样化、群像声音层层叠加）。
11. **`phone-and-crowd.md`** — 十一、手机与围观画面规则（手机作为环境元素、不遮挡主体）。
12. **`objects.md`** — 十二、物件规则（材质、位置、与人物动作绑定）。
13. **`scene.md`** — 十三、场景规则（稳定空间结构、背景服务人物）。
14. **`lighting.md`** — 十四、光影规则（时间统一、人物脸部重点、禁止项）。
15. **`psychological-montage.md`** — 十五、心理蒙太奇规则（拆分原则、快切镜头特征）。
16. **`sound-design.md`** — 十六、声音设计规则（默认无 BGM、主观心理变化技法、L-CUT/J-CUT）。
17. **`templates/storyboard.template.md`** — 十七、固定分镜模板（时长/景别/运镜/角度/画面动作/下意识细微动作/全系声场/台词情绪/台词/逻辑重音/环境音/人物与空间/正负向提示词），你在输出内容时，必须在每一个分镜中都按照里面的模板进行填空输出。
18. **`core-principles.md`** — 十八、最终核心原则（8 条核心原则与因果链路）。
19. **`prompt-optimization.md`** — 十九、提示词优化规则（保留情绪表达、逻辑重音标注、潜台词与台词区分、剧本咬合、台词不增不减）。
20. **`given-circumstances.md`** — 二十、规定情境分析规则（外部规定情境、内部规定情境、分析输出格式）。
21. **`core-axiom.md`** — 二十一、核心分析公理与人物关系情绪（情境催生一切、人物关系决定情绪表达、性格分析驱动情绪浓度）。
22. **`emotion-concentration.md`** — 二十二、CDS2.0 情绪浓度值体系（基础八大情绪、中层复合情绪、极致潜意识微情绪，共 36 个情绪）。
23. **`dialogue-processing.md`** — 二十三、台词处理规则（情绪语气色彩、重音处理、台词不增不减）。
24. **`body-language.md`** — 二十四、肢体动作规则（肢体动作分类、与情绪浓度匹配、与物件结合）。
25. **`shot-design-layers.md`** — 二十五、分镜设计三层级原则（叙事层、情绪层、镜头衔接层）。
26. **`workflow.md`** — 使用工作流（何时调用、如何套用模板、如何校验、输出规范）。

在用户开始创作分镜之前，先确认其场景空间与人物关系已建立，再按 `workflow.md` 的工作流套用模板。

---

## 本文件夹内容

```
seedance-storyboard-rules/
├── SKILL.md                          ← 你在这里（入口索引）
├── README.md                         ← 新用户快速入门
├── visual-rendering.md               ← 一、全局视觉渲染规则
├── shot-splitting.md                 ← 二、Seedance 2.0 单个视频的镜头拆分原则
├── shot-composition.md               ← 三、画面运作规则
├── spatial-continuity.md             ← 四、人物站位与物理空间连续性
├── shot-transitions.md               ← 五、电影级景别衔接规则
├── camera-movement.md                ← 六、镜头运动规则
├── acting.md                         ← 七、人物表演规则
├── subtext.md                        ← 八、人物潜台词规则
├── dual-layer-acting.md              ← 九、双层人物表演规则
├── ensemble.md                       ← 十、群像规则
├── phone-and-crowd.md                ← 十一、手机与围观画面规则
├── objects.md                        ← 十二、物件规则
├── scene.md                          ← 十三、场景规则
├── lighting.md                       ← 十四、光影规则
├── psychological-montage.md          ← 十五、心理蒙太奇规则
├── sound-design.md                   ← 十六、声音设计规则
├── core-principles.md                ← 十八、最终核心原则
├── prompt-optimization.md            ← 十九、提示词优化规则
├── given-circumstances.md            ← 二十、规定情境分析规则
├── core-axiom.md                     ← 二十一、核心分析公理与人物关系情绪
├── emotion-concentration.md          ← 二十二、CDS2.0 情绪浓度值体系
├── dialogue-processing.md            ← 二十三、台词处理规则
├── body-language.md                  ← 二十四、肢体动作规则
├── shot-design-layers.md             ← 二十五、分镜设计三层级原则
├── workflow.md                       ← 使用工作流
└── templates/
    └── storyboard.template.md        ← 十七、固定分镜模板，你在输出内容时，必须在每一个分镜中都按照里面的模板进行填空输出
```
