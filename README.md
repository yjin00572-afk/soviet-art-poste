# Soviet Aviation Poster

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111111?style=flat-square)](./SKILL.md)
[![Status](https://img.shields.io/badge/status-ready-2ea44f?style=flat-square)](#quick-start--快速开始)
[![Prompting](https://img.shields.io/badge/focus-image--to--poster-blue?style=flat-square)](#what-this-skill-returns--skill-输出内容)
[![Style](https://img.shields.io/badge/style-Soviet%20aviation%20poster-b31b1b?style=flat-square)](#design-rules--设计规则)
[![License](https://img.shields.io/badge/license-add%20your%20own-lightgrey?style=flat-square)](#license--许可证)
## 用途
> 将用户上传的图片改写为苏联民航海报风格，同时保留原图的可识别内容。  
> Transform uploaded images into Soviet civil aviation-era poster concepts while preserving the identity of the original scene.

这是一个 Codex skill，用来把用户上传的图片转换成“苏联民航海报”风格的提示词、构图方向和多语言广告文案。  
This is a Codex skill for turning uploaded images into Soviet civil aviation-style prompts, composition plans, and multilingual ad-copy directions.

它不是单纯做复古插画，而是强调两件事：保留原图内容，以及用中世纪后期苏联民航宣传海报的视觉语言重组画面。  
It is not just a retro illustration helper. Its job is to preserve the source image and rebuild it using the visual language of mid-century Soviet civil aviation posters.

## Quick Start / 快速开始

1. 将 skill 文件夹放入 Codex 的技能目录。  
   Put the skill folder inside your Codex skills directory.
   或者直接在codex、豆包等agent对话框中输入：请为我安装这个skill：https://github.com/yjin00572-afk/soviet-art-poste
   
2. 在 Codex 中上传一张图片。  
   Upload an image in Codex.
   
3. 调用 skill。  
   Invoke the skill with one of the templates below.
   提示词：
   1、Use $soviet-aviation-poster to transform my uploaded image into a Soviet-style poster.
   2、Use $soviet-aviation-poster to transform my uploaded image into a Soviet poster. 请先分析上传图里最独特的视觉锚点，并让它主导构图、配色和文案。请提取 3-6 个原图元素，把它们拆进拼贴结构里，避免每次都生成同一种海报。默认使用俄文、中文、英文三国语言，但文案必须直接描述上传图片里的地点、物体、建筑、季节、气氛或人物。若画面元素足够丰富，请使用 medium collage 或 high collage。

4.默认使用俄语、英语和中文，如果有不喜欢的可以二次调整。

## Examples Image / 示例图像
<img width="1365" height="2048" alt="image" src="https://github.com/user-attachments/assets/392569e6-94fd-43b0-8008-60da991e6dac" />
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/bfe3c94d-60bf-473f-9abd-fd893818cd81" />




### Install Location / 安装位置

默认路径：  
Default skill path:

```text
$CODEX_HOME/skills/soviet-aviation-poster
```

Windows 示例：  
Windows example:

```text
C:\Users\LENOVO\.codex\skills\soviet-aviation-poster
```

### Minimal Invocation / 简洁调用模板

```text
Use $soviet-aviation-poster to transform my uploaded image into a Soviet civil aviation poster. Analyze the image first, preserve the real subject, choose the best poster archetype, and return a full prompt, a short stable prompt, a negative prompt, and 3-5 multilingual headline options.
```

### Chinese Invocation / 中文调用模板

```text
Use $soviet-aviation-poster to transform my uploaded image into a Soviet civil aviation poster. 请先分析我上传图片里的主体、次要元素、情绪和最适合保留的视觉锚点，再输出：1. 风格判断 2. 选用的海报构图类型 3. 推荐配色 4. 完整长提示词 5. 稳定短提示词 6. 负面提示词 7. 3-5 个与图片内容相关的中俄英标题候选。注意最终画面必须和上传图片内容强相关，不要变成泛泛的飞机海报。
```

### Detailed Invocation / 详细调用模板

```text
Use $soviet-aviation-poster to transform my uploaded image into a Soviet civil aviation poster. Analyze the main subject, secondary motifs, mood, and visual anchors that must remain recognizable. Then return: 1) a style diagnosis, 2) a poster archetype, 3) a suggested palette, 4) a full art-director prompt, 5) a shorter stable prompt, 6) a negative prompt, and 7) 3-5 related headline options. Keep the final result strongly tied to the uploaded image rather than turning it into a generic airplane ad.
```
## 中文简介 / Chinese Overview

这个 skill 适合以下类型的任务：

- 风景图转旅行海报
- 城市夜景转航线广告
- 人像图转服务宣传海报
- 机场、桥梁、地标、街景转基础设施或目的地海报
- 餐饮、桌面、接待场景转“服务广告”风格海报

This skill works well for:

- landscape-to-travel-poster transformations
- skyline-to-route-advertisement transformations
- portrait-to-service-poster transformations
- terminals, bridges, landmarks, and streets turned into infrastructure or destination posters
- food, table, and hospitality scenes turned into service-advertisement posters


## Highlights / 亮点

- 根据上传图片自动选择更适合的海报构图 archetype  
  Chooses a poster archetype that matches the uploaded image
- 支持俄文、中文、英文文案方向  
  Supports Russian, Chinese, and English copy direction
- 包含文字安全模式，适合处理文字生成不稳定的模型  
  Includes text-safe guidance for models that render typography poorly
- 适合人像、天际线、海岸线、航站楼、桥梁、市场和接待场景  
  Works well for portraits, skylines, coastlines, terminals, bridges, markets, and hospitality scenes


## Examples / 示例

### Example 1: Night Skyline to Destination Poster / 夜景城市转目的地海报

Source image / 原图特征:

- harbor skyline
- bridge span
- deep blue sky
- building reflections

Recommended archetype / 推荐构图:

- `Night Illumination Poster`

Prompt direction / 提示词方向:

- preserve skyline and bridge identity
- use deep navy base with pale blue and vermilion accents
- add route arcs and light beams
- keep text to one headline and two labels

Possible headline directions / 标题方向:

- `Night Flight to the Harbor`
- `Gateway by Air`
- `Harbor Arrival`

### Example 2: Coastline to Route-Map Collage / 海岸线转路线拼贴海报

Source image / 原图特征:

- shoreline
- sea
- harbor or island forms
- travel mood

Recommended archetype / 推荐构图:

- `Route Map Collage`

Prompt direction / 提示词方向:

- split the scene into map sectors and route blocks
- use cobalt, faded cyan, ivory, and red accent
- add nodes, arcs, and one simplified aircraft cue

Possible headline directions / 标题方向:

- `Across the Blue Route`
- `Fly to the Northern Shore`
- `Coastal Service`

### Example 3: Portrait to Service Advertisement / 人像转服务宣传海报

Source image / 原图特征:

- person
- notable pose
- clothing silhouette
- hospitality or travel feel

Recommended archetype / 推荐构图:

- `Hero Figure Poster`
- or `Service and Hospitality Poster`

Prompt direction / 提示词方向:

- enlarge the figure
- use circular framing
- add a secondary skyline, meal, or route element
- keep typography short and welcoming

Possible headline directions / 标题方向:

- `At Your Service`
- `Air Road to Comfort`
- `Welcome Aboard`



## File Structure / 文件结构

```text
soviet-aviation-poster/
|- SKILL.md
|- README.md
|- agents/
|  `- openai.yaml
`- assets/
   `- examples/
      `- .gitkeep
```

## Validation / 校验

这个 skill 已通过 Codex skill validator 检查。  
This skill was validated with the Codex skill validator:

```text
python C:/Users/LENOVO/.codex/skills/.system/skill-creator/scripts/quick_validate.py C:/Users/LENOVO/.codex/skills/soviet-aviation-poster
```


## License / 许可证

本仓库默认使用 MIT License，详见 [LICENSE](./LICENSE)。  
This repository uses the MIT License. See [LICENSE](./LICENSE).



