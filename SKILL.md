---
name: soviet-aviation-poster
description: Transform uploaded images into stylized Soviet civil aviation-era poster concepts and image-generation prompts. Use when Codex needs to restyle a user image as a mid-century Soviet airline advertisement, travel poster, airport poster, route-map collage, service poster, or geometric aviation graphic with relevant multilingual headline copy and period-inspired layout guidance.
---

# Soviet Aviation Poster

Transform the user's uploaded image into a Soviet civil aviation poster aesthetic: limited but striking colors, flattened shapes, geometric abstraction, diagonal motion, assertive collage structure, print texture, and bold multilingual typography tied to the image content.

## Workflow

1. Analyze the uploaded image before writing the prompt.
2. Extract 3-6 recognizable motifs that must survive stylization.
3. Choose one poster archetype that matches the image.
4. Select one image-specific narrative angle that should control both composition and copy.
5. Build a constrained palette, collage plan, geometry plan, and text plan from the uploaded image rather than from a default airline template.
6. Write one high-control prompt and one fallback prompt.
7. Write one negative prompt.
8. Write 3-5 headline candidates tied to the uploaded content.
9. If exact text matters, prefer reserved text zones and short labels over dense copy.
10. Unless the user asks for a cleaner layout, prefer medium-to-high collage density rather than a single uninterrupted scene.
11. Unless the user explicitly asks for airline branding, keep the result airline-neutral and company-neutral.

## Analyze the image

Identify these elements from the uploaded image:

- Primary subject: person, building, coastline, mountain, street, vehicle, aircraft, skyline, bridge, harbor, market, landmark
- Secondary motifs: trees, sea, clouds, windows, towers, rails, signs, water reflections, vehicles, birds
- Scene logic: portrait, destination, city, infrastructure, resort, night view, transport, seasonal landscape
- Mood: heroic, optimistic, elegant, modernist, leisurely, industrial, festive, nocturnal
- Motion cue: ascent, glide, route line, spotlight, wind, speed streak, diagonal perspective, beam, orbit
- Best crop: portrait poster, square poster, wide poster
- Image anchors that must remain recognizable: clothing, roofline, skyline silhouette, shoreline, tower shape, bridge span, facade rhythm
- Primary differentiator: the one thing this image has that another upload would not share
- Best narrative angle: destination, architecture, portrait, hospitality, market life, weather, night mood, monumentality, leisure, infrastructure
- Text-worthy nouns: place names, landmark types, objects, seasons, colors, foods, signs, water, hills, towers, windows, boats, trees, streets

Preserve recognizability. The final poster must still clearly relate to the uploaded image rather than becoming a generic plane poster.

## Style grammar

Apply these rules unless the user asks otherwise.

### Color

Use 3-5 dominant colors.

- Prefer muted base tones with one vivid accent.
- Favor combinations such as:
  - faded cyan, cream, navy, vermilion
  - olive, dusty blue, ivory, brick red
  - teal, butter yellow, off-white, black
  - cobalt, pale sky blue, white, warm red
  - slate blue, sand, dark brown, faded orange
- Avoid full-spectrum realism, glossy gradients, neon overload, and modern HDR contrast.

### Form

- Flatten the scene into poster graphics rather than realistic rendering.
- Reduce detail into planes, silhouettes, cutout blocks, route arcs, circles, wedges, stripes, and diagonal bands.
- Use geometric background scaffolding: angled lines, radial rings, map fragments, gridded diagonals, spotlight beams, framed ovals, route nodes, poster borders.
- Prefer collage logic by default: split key image elements into separate zones or color fields rather than keeping one continuous scene.
- Reframe the image as assembled poster pieces: inset frames, clipped circles, cropped detail windows, route-map sectors, overlapping paper blocks, and separated image-derived fragments.
- When the source image has enough usable motifs, distribute at least 2-4 of them into different geometric compartments.
- Emphasize speed and direction with diagonals, contrails, route lines, or sweeping curves.

### Collage intensity

Use one of these modes:

- `light collage`: mostly one scene, with 1-2 inset panels or route fragments
- `medium collage`: default; main subject plus 2-4 supporting fragments in separate shapes
- `high collage`: aggressive montage; multiple cutout panels, inset destinations, cropped motifs, route sectors, and layered geometry

If the user says "more collage", "more montage", "more cutout", or "more poster assembly", switch to `high collage`.

### Texture

- Use subtle paper grain, offset print feel, mild ink fade, and slightly aged poster surfaces.
- Keep texture secondary to composition.
- Avoid heavy distress, torn paper excess, or dirty grunge unless the user explicitly asks for it.

### Typography

- Use bold sans-serif headline typography integrated into the composition.
- Place the main headline at the top, bottom, or vertically along one edge.
- Use smaller supporting text in three languages by default: Russian, Chinese, and English.
- Keep text short and functional: destination, scene identity, landmark, season, time of day, hospitality cue, or mood.
- Unless the user explicitly requests a real historical airline brand, do not use airline names, airline logos, route numbers, or company slogans.
- The three-language text must describe the uploaded image content rather than generic aviation copy.

### Variation and specificity

- Do not reuse the same poster logic for every image.
- Let one image-specific differentiator drive the composition. Examples: a harbor curve, a tower silhouette, a food tray, a winter tree line, a market awning, a night reflection, a human pose.
- If two prompts could swap source images without major changes, the prompt is too generic and must be rewritten.
- Derive the palette from the uploaded image first. Do not default to the same blue-red airline palette unless the source image genuinely supports it.
- Use at least 2 concrete nouns from the uploaded image in the headline and support-line planning.
- If the image contains no aviation object, keep the aviation influence in the graphic language only, not in the literal text subject.

### Airline-neutral copy rule

- Default to poster copy about the uploaded scene, not about an airline.
- Do not mention Aeroflot, Soviet Airlines, flight numbers, airline service, or aviation companies unless the user explicitly asks for that branding.
- Do not invent airports, aircraft, crews, or airline slogans when those ideas are absent from the uploaded image.
- The output may still feel like a Soviet travel poster, but the wording should center the real scene, object, place, or mood from the upload.

## Poster archetypes

Choose the closest archetype based on the uploaded image.

### 1. Hero Figure Poster

Use when the image contains a person, portrait, or strong human pose.

- Enlarge the figure.
- Place the person against an oval, disc, or diagonal color field.
- Add a secondary aircraft, skyline, or service element.
- Use a welcoming, service-oriented, or aspirational headline.

### 2. Route Map Collage

Use when the image contains geography, travel context, city landmarks, coastline, islands, roads, or multiple scene elements.

- Convert the composition into map-like blocks or sectors.
- Add directional lines, nodes, arcs, arrows, and labeled zones.
- Insert one simplified aircraft or travel icon crossing the layout.
- Prefer at least 3 distinct collage compartments when the source image supports them.

### 3. Aircraft and Landmark Poster

Use when the image contains architecture, monuments, skyline silhouettes, or a clear destination identity.

- Stylize the architecture into flat linework and color planes.
- Combine one aircraft with one or two iconic structures from the uploaded image.
- Use vertical scale and strong contrast.

### 4. Airport Infrastructure Poster

Use when the image has terminals, roads, vehicles, industrial forms, bridges, glass facades, cranes, or modernist geometry.

- Break the scene into blocks, windows, runways, shadows, and vehicles.
- Use sunrise, dusk, or spotlight geometry.
- Let the building shape carry the composition.

### 5. Seasonal Travel Poster

Use when the image suggests snow, sea, sunshine, forest, flowers, or atmospheric destination mood.

- Simplify the setting into emblematic symbols.
- Add one aircraft in motion.
- Let color and weather cues drive the theme.

### 6. Service and Hospitality Poster

Use when the image includes food, hotel-like interiors, tables, fashion, hospitality, or leisure cues.

- Keep one human or service object dominant.
- Frame supporting items as inset collage pieces.
- Use a clean service-promise headline.

### 7. Night Illumination Poster

Use when the image has night sky, city lights, reflections, lit buildings, or dramatic beams.

- Use deep blue or dark field backgrounds with one warm or bright accent.
- Add rings, arcs, beams, stars, or speed streaks.
- Keep the composition spacious and graphic.

## Palette selection by scene

Use these pairings as defaults.

- Sea or harbor: cobalt, faded cyan, ivory, red accent
- Forest or mountain: olive, dark teal, cream, warm red
- City architecture: dusty blue, stone, charcoal, pale yellow
- Night skyline: deep navy, pale blue, off-white, vermilion
- Snow or winter: pale sky, white, steel blue, red accent
- Food or hospitality: black, cream, pale blue, tomato red, apple green
- Desert or warm city: sand, faded turquoise, rust, dark brown

## Prompt assembly

Write prompts in this order:

1. Subject preservation
2. Poster era and medium
3. Chosen archetype
4. Geometry, collage density, and composition
5. Palette
6. Copy and typography
7. Texture and print finish

Always mention that the uploaded image content must remain recognizable.

## Prompt blocks

Use these reusable blocks to construct prompts.

### Subject preservation block

```text
Preserve the recognizable subject matter from the uploaded image, especially [anchors], and keep the final poster unmistakably tied to the original scene rather than replacing it with a generic aviation illustration.
```

### Era block

```text
Render it as a Soviet civil aviation poster from the 1950s-1980s, using flat graphic simplification, posterized shapes, restrained print colors, and a vintage travel-advertisement feel.
```

### Geometry block

```text
Recompose the scene with strong geometric abstraction, diagonal motion, assertive collage-like layering, route arcs, concentric circles, map fragments, inset frames, cropped motifs, bold negative space, and clean structural alignment.
```

### Collage block

```text
Break the uploaded scene into a poster montage rather than a single continuous image. Use [collage mode] with layered compartments, clipped circular crops, geometric panels, inset detail frames, overlapping paper shapes, and separated image-derived fragments that still preserve the original scene identity.
```

### Copy block

```text
Add a large integrated headline in bold sans-serif style and smaller secondary labels in Russian, Chinese, and English that directly reference the uploaded image content, place, object, season, architecture, or mood. Keep the wording airline-neutral unless the user explicitly requests airline branding.
```

### Texture block

```text
Finish with subtle paper grain, mild ink fade, and a printed poster surface rather than glossy digital realism.
```

## Comprehensive prompt templates

Use these when the user wants a stronger prompt set.

### 1. Full art-director prompt

```text
Transform the uploaded image into a stylized Soviet civil aviation poster from the 1950s-1980s. Preserve the recognizable subject matter from the uploaded image, especially [primary subject], [secondary motifs], and [visual anchors]. Recompose the scene as a flat graphic travel advertisement using the [chosen archetype] archetype, with [collage mode] collage density, strong geometric abstraction, diagonal motion, assertive collage-like layering, route arcs, framed color panels, inset fragments, concentric rings, and bold negative space.

Use a restrained palette of [palette], with low-to-moderate saturation and one vivid accent. Replace photographic realism with simplified silhouettes, cut-paper forms, architectural line reduction, posterized shadows, cropped image compartments, and clean shape hierarchies. Keep the uploaded scene identifiable while making it feel dynamic, elegant, optimistic, modernist, and visibly assembled from layered poster fragments.

Add a large integrated headline in a bold sans-serif style, plus smaller bilingual or trilingual labels in Russian, Chinese, and English that directly match the uploaded content: [headline direction], [supporting direction]. Keep typography functional, short, and tied to the actual uploaded subject rather than a default airline slogan. Apply subtle paper grain, offset-print feel, mild ink fade, and a mid-century poster finish.
```

### 2. Text-safe prompt

```text
Transform the uploaded image into a Soviet aviation poster while preserving the real subject, key landmarks, and scene identity. Use flat geometric simplification, diagonal energy, limited print colors, and a mid-century travel-ad aesthetic. Reserve clean text areas for one large headline and 2-3 short labels only. Use short Russian, Chinese, and English text related to the uploaded image itself, not to a generic airline. Avoid dense copy. Vintage paper texture, graphic composition, strong readability.
```

### 3. Collage-heavy prompt

```text
Rebuild the uploaded image as a high-collage Soviet route poster. Preserve the real content from the image, but split the subject into layered panels, map fragments, circles, route lines, inset frames, cropped detail windows, overlapping paper shapes, and diagonal color fields. Use clear montage logic with 3-5 separate visual compartments derived from the uploaded image. Limited palette, flat print graphics, aviation-era optimism, concise multilingual labels tied to the actual location or subject shown in the upload rather than to an airline brand.
```

### 6. High-collage mode prompt

```text
Transform the uploaded image into a high-collage Soviet civil aviation poster. Preserve the real subject and visual anchors from the source image, but reconstruct them as a montage of cutout panels, clipped circles, route-map sectors, inset detail frames, overlapping paper blocks, and cropped architectural or landscape fragments. The result should feel intentionally assembled, graphic, and poster-like rather than like one continuous flat illustration. Limited print palette, diagonal motion, multilingual labels tied to the source scene, vintage paper texture.
```

### 4. Minimal stable prompt

```text
Turn the uploaded image into a Soviet civil aviation travel poster. Keep the original subject recognizable. Flatten it into geometric color planes, diagonal motion, bold sans-serif typography, limited mid-century print colors, and subtle vintage paper texture. Add short Russian, Chinese, and English text related to the uploaded image.
```

### 5. Image-to-advertisement prompt

```text
Convert the uploaded photo into a stylized advertisement poster in a Soviet airline-era visual language. Preserve the actual content of the image, simplify it into flat graphics and collage geometry, and present it as an aspirational destination, scene, or hospitality poster with concise multilingual copy tied to the uploaded content, strong composition, and aged print texture.
```

## Scene-specific prompt recipes

Use one of these when the image clearly matches the scene.

### Scenic destination

```text
Turn the uploaded landscape or coastline image into a Soviet aviation travel poster. Preserve the actual landforms, waterline, horizon, and destination identity from the image, but flatten them into geometric color planes, diagonal motion lines, map-like framing, and limited mid-century print colors. Add a bold Russian headline plus smaller Chinese and English destination text tied to the scene. Elegant, dynamic, flat, slightly faded paper texture.
```

### Person-centric advertisement

```text
Transform the uploaded portrait or figure into a Soviet airline-era service poster. Keep the person's pose, silhouette, and notable clothing recognizable, enlarge the figure, place them against a circular or diagonal graphic field, and add simplified travel elements derived from the uploaded image. Limited palette, bold sans-serif headline, short multilingual side text, optimistic mid-century aviation mood.
```

### Architecture and infrastructure

```text
Rework the uploaded building, terminal, bridge, or city image as a Soviet civil aviation poster with strong geometric abstraction. Simplify the architecture into flat blocks, windows, shadows, structural lines, and diagonals, add one aircraft or route line, and integrate concise Russian, Chinese, and English poster text related to the specific location. Limited palette, print texture, bold modernist composition.
```

### Night travel

```text
Transform the uploaded night scene into a Soviet aviation poster with deep blue fields, bright geometric accents, route arcs, light beams, stars or speed streaks, and flat poster graphics. Preserve the real skyline, lighting pattern, and architectural anchors from the image. Add a short multilingual headline tied to the destination or night-travel mood.
```

### Food and hospitality

```text
Convert the uploaded food, table, or hospitality image into a Soviet civil aviation service poster. Keep the recognizable meal, serving objects, or service gestures from the original image, but stylize them into flat graphic shapes with strong contrast, circular framing, and a clean service-oriented layout. Add a short headline and brief multilingual labels related to onboard service, destination dining, or travel comfort.
```

### Market or street scene

```text
Turn the uploaded street, market, or urban-life scene into a Soviet travel poster while preserving the specific stalls, facades, signs, vehicles, and human flow from the photo. Use collage blocks, inset scene fragments, route-like diagonals, limited colors, and bold integrated type to frame the scene as a destination advertisement.
```

## Copy generation rules

Generate copy from the uploaded image, not from a generic airline theme.

### Headline logic

Create one short main line:

- 2-6 words in English or transliterated Russian
- or 4-10 Chinese characters
- or a bilingual pairing

Base the headline on one of these angles:

- destination promise
- scene identity
- heroic movement
- seasonal invitation
- landmark identity
- architectural monumentality
- daily-life vignette
- hospitality cue
- modern city optimism
- nocturnal atmosphere

## Explicit collage request handling

If the user explicitly asks for more collage:

- choose `Route Map Collage` unless another archetype is clearly better
- set collage mode to `high collage`
- increase the number of discrete compartments, insets, and cropped fragments
- mention montage, cut-paper assembly, inset panels, and separated image-derived pieces in the positive prompt
- avoid overly clean single-scene compositions
- still preserve the source image identity and anchors

### Headline formulas

Use formulas such as:

- `[Destination] in Color`
- `[Landmark] at Dusk`
- `To the [coast, peaks, harbor, towers]`
- `[Season] over [destination]`
- `[Harbor, Market, Garden, Square] by Morning`
- `Blue Night, [destination]`
- `Windows of [destination]`
- `[Bridge, Coast, Tower, Garden] Route`
- `[Food, Harbor, Square, Skyline] for the Journey`

### Supporting lines

Add 1-3 short supporting lines:

- destination or place line
- object or landmark cue
- seasonal cue
- time-of-day cue
- hospitality or comfort cue when the image supports it
- movement cue based on the picture, such as wind, water, lights, ascent, road, or crowd flow

Examples:

- `MOSCOW - HARBOR CITY`
- `Evening Lights over the River`
- `Stone Tower, Blue Horizon`
- `Summer Market, Red Awnings`
- `Modern Facade, Glass Rhythm`

### Multilingual rule

- Use Russian, Chinese, and English by default unless the user requests fewer languages.
- Make all three languages point to the same uploaded-image subject, not three unrelated slogans.
- Use Russian for period flavor, Chinese for compact vertical or side labeling, and English for a clean support line.
- If the uploaded image suggests a place, object, food, season, architecture, or mood, let that noun appear across the three-language set.
- Keep smaller text concise. Short labels are more stable than long paragraphs.
- Avoid generic words like `airline`, `flight`, `service`, `air route`, or `aviation` unless the uploaded image truly supports that topic.
- If the model is weak at text, use transliterated placeholders such as `[Russian headline]` and `[Chinese side label]` during image generation, then add exact text in a second step.

## Text fidelity rule

Image models often distort multilingual typography. If the user wants legible text:

- prioritize one large headline and a few short labels
- avoid long schedules or dense poster copy
- reserve clean blank zones for typography
- if needed, generate the poster with approximate type placement first, then add exact typography in a second design step

## Negative prompts

Use the base negative prompt, then add scene-specific exclusions when needed.

### Base negative prompt

```text
Avoid photorealism, glossy 3D rendering, modern corporate ad style, random futuristic UI, excessive gradients, painterly brushwork, cluttered composition, dense unreadable paragraphs, comic-book style, anime style, cyberpunk lighting, plastic textures, modern stock-photo look, unrelated symbols, irrelevant aircraft interiors, warped anatomy, broken perspective, and text that is detached from the image subject.
```

### Add when people are present

```text
Avoid distorted hands, extra fingers, asymmetrical eyes, melted facial structure, fashion-magazine glamour retouching, and modern beauty campaign styling.
```

### Add when architecture is present

```text
Avoid warped buildings, impossible window perspective, floating structures, overly realistic glass reflections, and futuristic skyscraper redesigns not present in the original image.
```

### Add when typography matters

```text
Avoid dense paragraphs, tiny body text, overlapping letters, decorative scripts, random lorem ipsum, and logos unrelated to the uploaded content.
```

## Response format

When using this skill, deliver:

1. One-sentence style diagnosis of the uploaded image
2. Chosen archetype
3. Suggested palette
4. One full art-director prompt
5. One shorter stable prompt
6. One negative prompt
7. Three to five headline candidates tied to the uploaded content
8. Optional note on text safety if the composition needs reserved text zones
9. If collage mode is medium or high, state which motifs should become separate inset pieces
10. State which uploaded-image differentiator drove the archetype, palette, and trilingual copy so the result does not collapse into a generic template

Do not give only generic style advice. Produce prompts that are immediately usable for image generation and clearly tied to the uploaded image.
