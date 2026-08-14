# Soviet Aviation Poster

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111111?style=flat-square)](./SKILL.md)
[![Status](https://img.shields.io/badge/status-ready-2ea44f?style=flat-square)](#quick-start--快速开始)
[![Prompting](https://img.shields.io/badge/focus-image--to--poster-blue?style=flat-square)](#what-this-skill-returns--skill-输出内容)
[![Style](https://img.shields.io/badge/style-Soviet%20aviation%20poster-b31b1b?style=flat-square)](#design-rules--设计规则)
[![License](https://img.shields.io/badge/license-add%20your%20own-lightgrey?style=flat-square)](#license--许可证)

> 将用户上传的图片改写为苏联民航海报风格，同时保留原图的可识别内容。  
> Transform uploaded images into Soviet civil aviation-era poster concepts while preserving the identity of the original scene.

这是一个 Codex skill，用来把用户上传的图片转换成“苏联民航海报”风格的提示词、构图方向和多语言广告文案。  
This is a Codex skill for turning uploaded images into Soviet civil aviation-style prompts, composition plans, and multilingual ad-copy directions.

它不是单纯做复古插画，而是强调两件事：保留原图内容，以及用中世纪后期苏联民航宣传海报的视觉语言重组画面。  
It is not just a retro illustration helper. Its job is to preserve the source image and rebuild it using the visual language of mid-century Soviet civil aviation posters.

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

默认输出包括：

1. 图片风格判断
2. 适合的海报构图类型
3. 推荐配色
4. 完整长提示词
5. 稳定短提示词
6. 负面提示词
7. 3-5 个和图片内容相关的标题候选

Default output includes:

1. A style diagnosis
2. A recommended poster archetype
3. A suggested palette
4. A full long-form prompt
5. A shorter stable prompt
6. A negative prompt
7. Three to five headline candidates tied to the uploaded image

## Banner Copy / Banner 文案

可用于 GitHub 社交预览、仓库副标题或首页顶部说明。  
Use these for your GitHub social preview, repository subtitle, or homepage callout.

### Short / 短版

`Turn any uploaded image into a Soviet aviation-style travel poster.`

### Long / 长版

`A Codex skill for converting real images into Soviet civil aviation-era poster prompts with geometric abstraction, limited palettes, multilingual copy, and strong source-image preservation.`

### Marketing / 宣传版

`From photo to propaganda-era travel poster: preserve the scene, rebuild the composition, and generate better prompts.`

## Highlights / 亮点

- 保留原图身份，不会把图像简单替换成泛泛的飞机海报  
  Preserves the identity of the original image instead of replacing it with a generic airplane poster
- 根据上传图片自动选择更适合的海报构图 archetype  
  Chooses a poster archetype that matches the uploaded image
- 输出完整 prompt、稳定短 prompt、负面 prompt 和标题候选  
  Produces a full prompt, a short stable prompt, a negative prompt, and headline candidates
- 支持俄文、中文、英文文案方向  
  Supports Russian, Chinese, and English copy direction
- 包含文字安全模式，适合处理文字生成不稳定的模型  
  Includes text-safe guidance for models that render typography poorly
- 适合人像、天际线、海岸线、航站楼、桥梁、市场和接待场景  
  Works well for portraits, skylines, coastlines, terminals, bridges, markets, and hospitality scenes

## Effect Gallery / 效果图展示

发布到 GitHub 时，可在这里放置前后对比图。  
When publishing to GitHub, place your before-and-after examples here.

```md
## Effect Gallery

| Source | Poster Result |
| --- | --- |
| ![Source 1](./assets/examples/harbor-night-source-v1.jpg) | ![Poster 1](./assets/examples/harbor-night-poster-v1.jpg) |
| ![Source 2](./assets/examples/portrait-service-source-v1.jpg) | ![Poster 2](./assets/examples/portrait-service-poster-v1.jpg) |
```

推荐展示组合：  
Recommended showcase sets:

- portrait -> service poster
- skyline -> night flight poster
- coastline -> route map collage
- terminal or bridge -> infrastructure poster
- food or hospitality scene -> service advertisement

## Quick Start / 快速开始

1. 将 skill 文件夹放入 Codex 的技能目录。  
   Put the skill folder inside your Codex skills directory.
2. 在 Codex 中上传一张图片。  
   Upload an image in Codex.
3. 用下方模板调用 skill。  
   Invoke the skill with one of the templates below.
4. 把返回的 prompt 复制到你的出图模型里，或当作二次艺术指导 prompt 使用。  
   Copy the returned prompt into your image model, or use it as a second-pass art-direction prompt.
5. 如果文字变形严重，改用 text-safe 模板，或分两步加字。  
   If text is distorted, use the text-safe template or add typography in a second step.

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

### Text-Safe Invocation / 文字安全模式调用

```text
Use $soviet-aviation-poster to turn my uploaded image into a text-safe Soviet poster. Prioritize composition and subject preservation, keep typography to one large headline and 2-3 short labels, and return a long prompt, short prompt, negative prompt, and headline candidates.
```

## What This Skill Returns / Skill 输出内容

预期输出格式：  
The intended response format is:

1. 一句话风格判断 / One-sentence style diagnosis
2. 选用的海报 archetype / Chosen poster archetype
3. 推荐配色 / Suggested palette
4. 完整长提示词 / One full art-director prompt
5. 稳定短提示词 / One shorter stable prompt
6. 负面提示词 / One negative prompt
7. 3-5 个标题候选 / Three to five headline candidates
8. 可选的文字安全提示 / Optional text-safety note

## Best Use Cases / 适用场景

适合把上传图片转换为：  
Use this skill when you want to transform an uploaded image into:

- 苏联民航风格旅行海报 / a Soviet airline-style travel poster
- 目的地广告 / a destination advertisement
- 路线拼贴海报 / a route-map collage poster
- 机场或基础设施海报 / an airport or infrastructure poster
- 餐饮或服务宣传海报 / a hospitality or service poster
- 夜航或季节旅行海报 / a night-flight or seasonal travel poster

典型原图类型：  
Typical source images:

- portraits
- skylines
- coastlines
- terminals
- bridges
- landmarks
- urban night scenes
- hospitality scenes
- streets and markets

## Design Rules / 设计规则

### Preserve Recognizability / 保留可识别性

最终结果必须和原图保持明确关联。  
The final result should remain clearly related to the uploaded image.

应优先保留这些锚点：  
Keep anchors such as:

- skyline silhouette
- shoreline
- bridge span
- building rhythm
- clothing silhouette
- pose
- landmark outline
- lighting pattern

如果这个 prompt 换任何图片都能用，那就说明它太泛化了。  
If the result could work with any other source image, the prompt is too generic.

### Use Limited but Striking Color / 用有限但醒目的色彩

推荐行为：  
Preferred behavior:

- 3-5 dominant colors
- low-to-moderate saturation
- one vivid accent
- poster-like contrast

避免：  
Avoid:

- HDR realism
- glossy gradients
- neon overload
- modern corporate polish

### Build with Geometry / 用几何结构搭画面

优先使用：  
Use:

- diagonal bands
- circles
- route arcs
- framed panels
- map fragments
- beams
- rings
- blocks of negative space

### Keep Text Functional / 让文字服务构图

推荐文字策略：  
Preferred text behavior:

- one large headline
- 2-3 short support labels
- Russian as the main flavor
- Chinese and English as secondary support when appropriate

避免：  
Avoid:

- dense paragraphs
- long schedules
- tiny text
- decorative scripts

## Poster Archetypes / 海报构图类型

### 1. Hero Figure Poster / 人物主视觉海报

适合人像、服务人员、姿态强烈的人物。  
Best for portraits, service staff, and strong human poses.

### 2. Route Map Collage / 路线拼贴海报

适合海岸线、地理信息、城市组团和旅行场景。  
Best for coastlines, geography, city clusters, and travel context.

### 3. Aircraft and Landmark Poster / 飞机与地标海报

适合纪念性建筑、天际线和目的地识别度强的图片。  
Best for monuments, skylines, and strong destination identity.

### 4. Airport Infrastructure Poster / 机场基础设施海报

适合航站楼、道路、桥梁、起重机和现代主义结构。  
Best for terminals, roads, cranes, bridges, and modernist structures.

### 5. Seasonal Travel Poster / 季节旅行海报

适合海景、雪景、森林、花卉和气候明显的场景。  
Best for sea, snow, forest, flowers, and climate-led scenes.

### 6. Service and Hospitality Poster / 服务广告海报

适合食物、桌面、室内空间和接待感明显的场景。  
Best for food, tables, interiors, and leisure cues.

### 7. Night Illumination Poster / 夜间灯光海报

适合夜景、反光、灯带、光束和戏剧化照明。  
Best for night skylines, lit buildings, reflections, and dramatic beams.

## Default Palette Suggestions / 默认配色建议

- Sea or harbor / 海港海岸: `cobalt, faded cyan, ivory, red accent`
- Forest or mountain / 森林山地: `olive, dark teal, cream, warm red`
- City architecture / 城市建筑: `dusty blue, stone, charcoal, pale yellow`
- Night skyline / 夜间天际线: `deep navy, pale blue, off-white, vermilion`
- Snow or winter / 冬季雪景: `pale sky, white, steel blue, red accent`
- Food or hospitality / 餐饮服务: `black, cream, pale blue, tomato red, apple green`
- Desert or warm city / 暖色城市: `sand, faded turquoise, rust, dark brown`

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

## Prompt Skeleton / Prompt 骨架

```text
Transform the uploaded image into a stylized Soviet civil aviation poster from the 1950s-1980s. Preserve the recognizable subject matter from the uploaded image, especially [anchors]. Recompose the scene as a flat graphic travel advertisement using the [chosen archetype] archetype, strong geometric abstraction, diagonal motion, collage-like layering, route arcs, framed color panels, and bold negative space.

Use a restrained palette of [palette], with low-to-moderate saturation and one vivid accent. Replace photographic realism with simplified silhouettes, cut-paper forms, posterized shadows, and clean shape hierarchies.

Add a large integrated headline in bold sans-serif style, plus smaller Russian, Chinese, and English labels tied directly to the uploaded content. Keep typography short and functional. Finish with subtle paper grain, mild ink fade, and a printed poster surface rather than glossy digital realism.
```

## Text Rendering Notes / 文字渲染注意事项

多语言文字在图像模型里经常失真。  
Image models often distort multilingual text.

如果文字质量很重要：  
If text quality matters:

- keep copy short
- use one major headline
- use 2-3 short labels only
- reserve blank areas for later typography placement
- consider a two-step workflow:
  - generate the poster composition first
  - add exact text in a second design pass

## Negative Prompt Strategy / 负面提示词策略

默认负面 prompt 应抑制以下问题：  
The default negative prompt should suppress:

- photorealism
- glossy 3D rendering
- modern corporate ad style
- excessive gradients
- cluttered composition
- unreadable paragraphs
- cyberpunk lighting
- unrelated symbols
- broken anatomy
- broken perspective
- text unrelated to the image subject

按需追加排除项：  
Add extra exclusions when needed:

- people: distorted hands, asymmetrical faces, glamour-retouch look
- architecture: warped buildings, impossible windows, futuristic redesigns
- typography: overlapping letters, tiny body text, decorative scripts

## Assets and Naming Convention / 示例素材目录与命名规范

把示例素材放在这里：  
Create example assets under:

```text
assets/examples/
```

推荐目录结构：  
Recommended layout:

```text
assets/
`- examples/
   |- .gitkeep
   |- harbor-night-source-v1.jpg
   |- harbor-night-poster-v1.jpg
   |- coastline-route-source-v1.jpg
   |- coastline-route-poster-v1.jpg
   |- portrait-service-source-v1.jpg
   `- portrait-service-poster-v1.jpg
```

推荐命名格式：  
Recommended filename pattern:

```text
[theme]-[scene]-[kind]-v[version].[ext]
```

字段解释：  
Where:

- `theme`: 大类主题，如 `harbor`, `coastline`, `portrait`, `terminal`
- `scene`: 更具体的场景，如 `night`, `route`, `service`, `bridge`
- `kind`: `source`, `poster`, `detail`, or `mockup`
- `version`: `v1`, `v2`, `v3`
- `ext`: `jpg`, `png`, or `webp`

好示例：  
Good examples:

- `harbor-night-source-v1.jpg`
- `harbor-night-poster-v1.jpg`
- `terminal-bridge-source-v2.png`
- `terminal-bridge-poster-v2.png`
- `portrait-service-detail-v1.webp`

命名规则：  
Rules:

- use lowercase only
- use hyphens, not spaces
- keep source and result pairs identical except for `kind`
- increment the version when you materially change the image
- prefer `jpg` or `webp` for final showcase assets unless transparency matters

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

## Roadmap / 路线图

- [ ] Add real before-and-after sample images under `assets/examples/`
- [ ] Add English and Chinese prompt presets for common scene types
- [ ] Add a logo-safe mode for users who want generic period branding only
- [ ] Add second-pass typography templates for cleaner multilingual poster text
- [ ] Add a few curated benchmark source images and expected output directions
- [ ] Add optional output modes for SDXL, Flux, and image-editing workflows

## Contributing / 贡献方式

欢迎这类贡献：  
Good contributions include:

- new example prompts
- better before-and-after showcases
- more stable multilingual copy patterns
- additional archetypes that still preserve source-image identity
- tested prompt variants for specific image models

优先接受“让 prompt 更贴合原图”的改进，而不是更泛化的改动。  
When contributing, prefer improvements that make prompts more image-specific rather than more generic.

## License / 许可证

本仓库默认使用 MIT License，详见 [LICENSE](./LICENSE)。  
This repository uses the MIT License. See [LICENSE](./LICENSE).

## High-Collage Mode / 强拼贴模式

Use this mode when the default poster result is too clean, too flat, or not montage-like enough.

在默认结果拼贴感不够、画面过于完整、缺少切片和分区时，使用这个模式。

### High-Collage Invocation / 强拼贴调用模板

```text
Use $soviet-aviation-poster to transform my uploaded image into a high-collage Soviet civil aviation poster. Preserve the real subject and visual anchors from the source image, but make it much more montage-like, with inset frames, cropped detail windows, clipped circles, route-map sectors, overlapping paper blocks, and 3-5 separate visual compartments.
```

```text
Use $soviet-aviation-poster to transform my uploaded image into a Soviet civil aviation poster. 请加强拼贴感，使用 high collage 模式，把画面拆成多个几何拼贴块、局部裁切窗、圆形切片、路线图分区和叠压纸片结构，同时保留原图主体和视觉锚点。
```

### High-Collage Prompt Skeleton / 强拼贴 Prompt 骨架

```text
Transform the uploaded image into a high-collage Soviet civil aviation poster. Preserve the recognizable subject matter from the uploaded image, especially [anchors]. Rebuild the scene as an assembled poster montage instead of one continuous illustration, using [chosen archetype], strong geometric abstraction, inset frames, clipped circles, cropped detail windows, route-map sectors, overlapping paper blocks, and 3-5 separate visual compartments derived from the source image.

Use a restrained palette of [palette], with low-to-moderate saturation and one vivid accent. Replace photographic realism with simplified silhouettes, cut-paper forms, posterized shadows, cropped fragments, and clean shape hierarchy. Keep the source image identifiable while making the composition feel intentionally layered, graphic, dynamic, and visibly constructed from separate poster pieces.

Add a large integrated headline in bold sans-serif style, plus smaller Russian, Chinese, and English labels tied directly to the uploaded content. Keep typography short and functional. Finish with subtle paper grain, mild ink fade, and a printed poster surface rather than glossy digital realism.
```

### High-Collage Checklist / 强拼贴检查清单

- Use 3-5 separate visual compartments when the source image has enough motifs.
- Add inset frames, cropped windows, clipped circles, or route-map sectors instead of one uninterrupted scene.
- Keep the original subject identifiable even when the layout becomes more fragmented.
- Prefer medium-to-high collage density over a clean single-panel composition.
- Keep text short so the added montage structure remains readable.

## Variation Rules / 差异化生成规则

If your outputs look too similar, the usual problem is not the style reference. The usual problem is that the prompt keeps reusing the same archetype, the same palette logic, and the same headline logic across different uploads.

如果生成结果太像，通常不是“风格不够像”，而是每次都在复用同一种海报 archetype、同一种配色套路、同一种文案套路。

Use these rules:

- Let one image-specific differentiator control the poster.
- Extract 3-6 visible motifs from the uploaded image and force them into the composition.
- Choose the archetype from the image, not from habit.
- Derive the palette from the uploaded image first, then Sovietize it.
- Use medium or high collage when the image has enough secondary elements.
- Make the trilingual text describe the uploaded image content, not an airline.
- Do not mention airline brands, company names, route numbers, or airline slogans unless explicitly requested.

Recommended self-check:

- What is the most unique visual anchor in this upload?
- Is this image mainly architecture, portrait, market, night scene, coastline, hospitality, or infrastructure?
- Do the headline nouns really come from the uploaded image?
- If the same prompt could fit another upload with no major edits, it is still too generic.

### Content-First Trilingual Copy / 内容优先三语文案

Default language set:

- Russian
- Chinese
- English

But the text topic must come from the uploaded image:

- architecture -> landmark, tower, bridge, facade, skyline
- coastline -> coast, harbor, waves, horizon, pier
- market or street -> awnings, stalls, square, lights, crowd flow
- hospitality or food -> table, fruit, tea, service, comfort
- portrait -> pose, uniform, gesture, silhouette, gaze
- night scene -> moonlight, lamps, blue night, reflection, windows

Avoid default airline copy such as:

- `Aeroflot`
- `Soviet Airlines`
- `Flight Service`
- `Air Route`
- generic company slogans

Prefer content-linked copy such as:

- `Harbor at Dusk`
- `Blue Night, Odessa`
- `Summer Market`
- `Windows of the Coast`
- `Tower and River`

### Recommended Invocation / 推荐调用模板

```text
Use $soviet-aviation-poster to transform my uploaded image into a Soviet poster with stronger variation across different source images. Analyze the uploaded image first, identify the primary differentiator, extract 3-6 visual motifs, choose the best archetype from the image itself, and derive the palette from the image content rather than from a default airline palette. Use Russian, Chinese, and English text by default, but make all text directly about the uploaded image subject, place, object, architecture, season, or mood. Do not use airline brands, company names, or generic aviation slogans unless I explicitly ask for them. If the image contains enough secondary elements, use medium or high collage and split the scene into multiple image-derived compartments.
```

```text
Use $soviet-aviation-poster to transform my uploaded image into a Soviet poster. 请先分析上传图里最独特的视觉锚点，并让它主导构图、配色和文案。请提取 3-6 个原图元素，把它们拆进拼贴结构里，避免每次都生成同一种海报。默认使用俄文、中文、英文三国语言，但文案必须直接描述上传图片里的地点、物体、建筑、季节、气氛或人物，不要默认写航空公司、航线号、服务口号，除非我明确要求。若画面元素足够丰富，请使用 medium collage 或 high collage。
```
