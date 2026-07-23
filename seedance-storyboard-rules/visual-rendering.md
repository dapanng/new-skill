## 一、全局视觉渲染规则

### 视觉风格（非固定）

根据剧本题材、场景类型、人物设定选择最合适的视觉风格。可选项包括但不限于：

| 风格类型 | 适用场景 | 提示词参考 |
|----------|----------|------------|
| 高端 3D CG | 奇幻、科幻、游戏改编剧 | High-end cinematic 3D CG render, Final Fantasy CG style, semi-stylized 3D character |
| 真人写实 | 现实题材、都市情感、悬疑罪案 | Photorealistic, cinematic live-action, real skin texture |
| 2D 动漫 | 青春校园、热血、二次元题材 | 2D anime style, cel shading, Studio Ghibli inspired |
| 水彩/油画 | 古风、文艺、诗意题材 | Watercolor / oil painting style, soft brush strokes |
| 水墨 | 武侠、古风、东方题材 | Chinese ink painting style, sumi-e, traditional brushwork |
| 赛博朋克 | 近未来、科技、反乌托邦 | Cyberpunk style, neon lighting, futuristic aesthetic |
| 黏土/定格 | 童话、治愈、创意短片 | Claymation / stop-motion style, handmade texture |

### 风格选择原则

1. **风格服务于叙事与情绪**，不服务于炫技。
2. 一旦确定风格，**整组镜头必须统一**，不能中途切换。
3. 风格选择必须与规定情境（参考第二十节）匹配：
   - 时代、地点、环境决定风格基调
   - 人物身份、事件决定风格质感
4. 风格必须与情绪浓度值（参考第二十二节）匹配：
   - 高浓度情绪（75%+）→ 风格对比度强、光影戏剧化
   - 低浓度情绪（<35%）→ 风格柔和、光影平缓

### 默认风格提示词模板

确定风格后，将其填入正向提示词开头。以下是通用质量基底，可与任何风格叠加：

```
(Masterpiece, best quality, 8K resolution, cinematic composition:1.4)
```

具体风格提示词根据上述风格类型表选择，叠加在质量基底之后。

### 整体视觉要求（通用）

无论选择何种风格，均须保证：

- 电影级画面质感
- 统一的艺术风格基调
- 符合叙事与情绪需求

### 人物皮肤质感要求（按风格调整）

**3D CG / 真人写实风格**：

- 自然皮肤纹理
- 次表面散射
- 合理粗糙度
- 真实面部肌肉变化
- 细腻发丝
- 眼球湿润感
- 眼部高光
- 真实材质反射

**2D 动漫风格**：

- 干净线条
- 赛璐璐上色层次
- 简化但精准的阴影分区
- 眼神高光保留情绪表达

**水彩/水墨/油画风格**：

- 笔触质感统一
- 色彩层次符合材料特性
- 人物面部保留情绪可读性

### 禁止项

- 文字
- 字幕
- 水印

### 叙事视频声音默认

- **禁止 BGM**
- 只保留：对白、OS、环境音、动作音效、Foley 和必要的主观听觉设计

---
