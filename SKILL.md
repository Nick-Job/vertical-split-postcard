---
name: vertical-split-postcard
description: Create vertical split-composition matte-cream album postcards that keep a realistic photo on the top half and an ink-wash flat deconstruction illustration on the bottom half, with a thin elegant serif English title at the very bottom. Use when the user provides reference photos of scenery, architecture, temples, landmarks, or travel scenes and wants them converted into this two-part postcard style, or asks for 竖向二分构图/米白明信片/水墨扁平解构/画册明信片 images.
---

# Vertical Split Postcard

Turn one or more reference photos into a vertical split-composition matte-cream album postcard: realistic photo on top, independent cream negative space with a low-saturation ink-wash flat deconstruction illustration below, and a thin serif English title at the very bottom.

## Workflow

1. Read `references/prompt-spec.md` before composing.
2. Analyze every reference image. If the current model cannot read images directly, run the claude-vision-skill helper:
   `node /Users/jia/.codex/skills/claude-vision-skill/vision.js "<image path>" "describe subject, layout, palette, light, textures, and all visible elements in Chinese"`
   Extract for each image: subject and scene, main architecture or objects, palette families, light direction and contrast, textures, and title style.
3. Compose one final prompt per reference image using the prompt-spec order. Keep the original realistic photo unchanged in the prompt: do not let the generator merge, crop, re-light, or stylize the top half.
4. If the user asks for a series, keep the same paper, typography, and illustration language across all cards, but let each scene keep its own layout.
5. Generate with the available image generation tool. Pass the reference images as style and subject references when the tool supports input images.
6. Validate against the checklist below. Iterate with one targeted change at a time when a check fails.

## Validation checklist

- Vertical split: clear horizontal division; top is the unmodified realistic photograph, bottom is an independent cream blank area; the same subject appears in both halves.
- Top half: original scene layout, silhouettes, and native low-saturation colors are preserved; no stylization of the photo.
- Bottom half: flat geometric deconstruction, layered soft color blocks, ink-wash bleeding edges, no sharp hard outlines, no fine textures, no clutter, no photo lighting or shadows.
- Palette: bottom colors are drawn from the photo and softened into a low-saturation cream-and-earth palette; paper base is matte cream with subtle grain.
- Typography: one thin elegant serif English title centered at the very bottom, small and restrained; no gibberish text, no extra letters.
- Whitespace: large negative space, clean eastern architectural study layout, no extra decoration.

## References

- `references/prompt-spec.md`: fixed core prompt and final assembly rules.
- `references/examples.md`: worked examples adapted from real reference scenes.
