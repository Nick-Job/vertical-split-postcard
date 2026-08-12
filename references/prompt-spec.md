# Vertical Split Postcard Prompt Spec

Use the core prompt below as the fixed style base. Add a short subject block before it, insert the title into the final sentence, then append the avoid list. Keep this order.

## Core prompt (verbatim)

> 竖向二分构图哑光米白画册明信片，画面上半部分完整保留原图写实实拍风景，不改动景物布局、轮廓、原生低饱和配色；下半部分独立米色留白区域，水墨扁平解构插画，提取原图全部景物几何极简简化，分层柔和色块，毛笔淡墨晕染笔触，无锐利硬线条，复刻原图全部色彩调性，删除全部细碎纹理、杂物、光影；画面最底部添加纤细优雅衬线英文标题，整体米白哑光纸张底色，大面积留白，简约东方建筑风景研究版式，干净高级，无多余装饰。

## Subject block (lead-in)

- State that the attached image is the sole source: "以用户提供的原图为唯一参考：上半部分就是这张实拍照片本身，不做任何改图、裁剪、重打光或风格化。"
- Name the concrete scene in one sentence, e.g. "画面主体是带脊兽的深灰瓦面飞檐与红褐色檐底，背景为淡蓝天空和绿树。" Use only what is visible in the reference.
- Describe the bottom-half deconstruction in one sentence: which elements survive, reduced to their essential geometry (roof eaves, tower, pavilion, arch, statue silhouette, skybridge), and which are removed (window grids, railings, brick joints, leaves, visitors, glare).

## Title

- One thin elegant serif English word or short phrase, centered at the very bottom, dark gray, small size.
- Prefer meaningful text. When the user supplies a place, building, or series name, use that instead of invented gibberish.
- Optionally allow two short horizontal hairline accents flanking the title, as seen in the reference series; never add other typographic decoration.

## Final assembly order

1. Reference-image role statement.
2. Subject block (top half unchanged, bottom half deconstruction).
3. Core prompt verbatim, with the concrete title inserted in place of "纤细优雅衬线英文标题" when it is meaningful.
4. Avoid list: no extra decoration, no visible frames or borders, no watermark, no gradient, no sharp outlines, no thick or decorative fonts, no gibberish letters, no removing or adding scenery in the top half.

## Style invariants (from the reference series)

- Paper: matte cream throughout, subtle paper grain, warm off-white rather than pure white.
- Top half: hard daylight, clear shadows, native colors, full texture.
- Bottom half: Morandi-like low-saturation palette lifted from the photo, soft flat color blocks, wet ink bleeding at edges, at least half of the lower band left blank.
- Typography: thin serif, often italic, dark gray, small, at the very bottom center.
