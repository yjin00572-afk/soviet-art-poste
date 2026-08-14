# Soviet Aviation Poster

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111111?style=flat-square)](./SKILL.md)
[![Status](https://img.shields.io/badge/status-ready-2ea44f?style=flat-square)](#quick-start--快速开始)
[![Prompting](https://img.shields.io/badge/focus-image--to--poster-blue?style=flat-square)](#what-this-skill-returns--skill-输出内容)
[![Style](https://img.shields.io/badge/style-Soviet%20aviation%20poster-b31b1b?style=flat-square)](#design-rules--设计规则)
[![License](https://img.shields.io/badge/license-add%20your%20own-lightgrey?style=flat-square)](#license--许可证)
## 用途
> 这是一个 Codex skill，可将用户上传的图片改写为苏联海报风格，同时保留原图的可识别内容。  

感谢你的喜欢，第一次制作可能有一些问题，如果有任何问题或者灵感欢迎抖音艾特我 @Breathe 


## Quick Start / 快速开始

1. 将 skill 文件夹放入 Codex 的技能目录。  
   Put the skill folder inside your Codex skills directory.
   
   或者直接在codex、豆包等agent对话框中输入：请为我安装这个skill：https://github.com/yjin00572-afk/soviet-art-poste
   
3. 在 Codex 中上传一张图片。  
   Upload an image in Codex.
   
4. 调用 skill。  
   Invoke the skill with one of the templates below.
   提示词：
   >（1）Use $soviet-aviation-poster to transform my uploaded image into a Soviet-style poster.
   >（2）建筑/城市 专用空间版：
   >Use $soviet-aviation-poster to transform my uploaded image into a Soviet poster. 请优先保留建筑或城市的空间过渡感，先分析前景、中景、背景、地平线、天际线叠压、道路/桥梁/立面退深，再把这些空间关系压缩成海报化层次。不要把城市直接压成一张纯平贴片，要保留 2-3 层可读景深，可用建筑遮挡、尺度变化、远近明度、光束、窗口节奏和斜向透视来表现空间。颜色请先根据原图主色和冷暖关系决定，再做苏联风格化，不要套固定蓝红模板。默认俄文、中文、英文三语，文案必须直接对应图中的地点、建筑、时间感或气氛。
   >（3）人物/场景 专用空间版：
   >Use $soviet-aviation-poster to transform my uploaded image into a Soviet poster. 请优先保留人物与环境之间的空间关系，先分析人物是否在前景、后方是否有建筑/街道/天空/室内层次，再把前景人物、中景物件、背景环境压缩成海报化景深，而不是全部压成同一平面。请保留 2-3 层空间过渡，可用人物遮挡、桌面或栏杆前景、背景轮廓叠压、光带、远近色阶和局部拼贴窗来表现空间。颜色请根据原图主色、肤色、服装色和环境色来决定苏联风格化方案，不要固定配色。默认俄文、中文、英文三语，文案必须直接对应图中的人物、动作、物体、地点或氛围。
   

4.默认使用俄语、英语和中文，如果有不喜欢的可以二次调整。

## Examples Image / 示例图像
<img width="1365" height="2048" alt="image" src="https://github.com/user-attachments/assets/392569e6-94fd-43b0-8008-60da991e6dac" /><img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/bfe3c94d-60bf-473f-9abd-fd893818cd81" />





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



