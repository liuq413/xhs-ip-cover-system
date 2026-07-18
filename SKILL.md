---
name: xhs-ip-cover-system
description: Create reusable Xiaohongshu (小红书/XHS) cover and social-card systems around a personal IP character. Use when the user asks for a 小红书封面图、小红书卡片、文章配图、IP形象配图、Q版人物封面、个人品牌视觉、社交媒体封面, or asks to design, generate, package, document, standardize, or replace the sample character with their own IP style.
---

# XHS IP Cover System

Use this skill to create high-consistency Xiaohongshu cover concepts around a reusable personal IP character. It is designed for creators who want a repeatable visual system, not one-off pretty images.

## Core Rule

Build the cover from four layers:

1. **Content intent**: what the reader should understand or want.
2. **IP character**: the creator's repeatable visual spokesperson.
3. **Cover structure**: title, character, information blocks, and stickers.
4. **Style variant**: the visual mood selected for the content type.

Never treat the character as decoration. The character must make the content feel more recognizable, trustworthy, approachable, or memorable.

## Standard Workflow

1. Collect the cover brief.
2. Choose a character mode.
3. Choose or adapt a style variant.
4. Build the visual structure.
5. Write the generation prompt.
6. Generate one direction first.
7. Run thumbnail, character, and information-density checks.
8. Iterate or archive.

For the complete operational SOP, read `references/cover-production-sop.md`. Read `references/replace-with-your-ip.md` when the user provides or wants to replace an IP reference image.

## Brief Questions

Ask for missing information only when needed. Prefer these fields:

```text
Content type:
Main title:
Topic:
Reader promise:
Reusable framework or method:
Extra assets:
Character mode:
Style variant:
Mood:
Aspect ratio:
```

If the user asks for a quick demo, make reasonable assumptions and generate one image first.

If an image-generation tool is available, use it after the direction is confirmed. If no image-generation tool is available, return the complete prompt and a layout specification instead of claiming that an image was generated.

## Character Modes

Use a **professional mode** for:

- Method explainers
- Tool tutorials
- Case studies
- Product, course, or service promotion

Use a **friendly mascot mode** for:

- Beginner explainers
- Resource recommendations
- Light seeding
- Gentle warnings
- Recurring column covers

When the user needs to replace the sample character with their own IP, read `references/replace-with-your-ip.md`.

When the user provides multiple IP images, use the clearest front-facing image for facial identity, then use additional images only for outfit, hat, pose, or scene references. Do not merge conflicting facial traits without confirming which image is authoritative.

## Style Variants

The bundled reference system includes four example friendly-mascot variants:

- Cream Companion
- Black Efficiency
- Utility Fieldwork
- Street Sprint

For selection rules and visual traits, read `references/style-variants.md`.

## Prompting

Always include:

- Aspect ratio, usually `3:4`
- Main title text
- Character identity and fixed traits
- Layout structure
- Relevant stickers/cards/icons
- Negative constraints such as no watermark, no unrelated props, no extra characters
- A text-safe area when the image model is unreliable at rendering Chinese text

Use `references/prompt-templates.md` for prompt templates.

For Chinese titles longer than a short phrase, prefer a clean text-safe layout and add the final text in a design or post-processing tool. Keep the requested aspect ratio; `3:4` is the default for Xiaohongshu covers, not a universal requirement.

## Quality Checks

Before finalizing, verify:

- The title is readable in a small mobile feed.
- The character still looks like the same IP.
- The cover communicates one main idea.
- Information blocks support the topic.
- The style can become a series, not a one-off.
- The output dimensions and crop are correct for the requested ratio.

Use `references/quality-checklist.md` for the full checklist.

## Output Expectations

When delivering a result, include:

```text
Used:
- Content type:
- Character mode:
- Style variant:
- Main title:
- Aspect ratio:

Result:
- Image or prompt:
- Suggested next iteration:
- Archive path, if applicable:
```

## Bundled Resources

- `references/cover-production-sop.md`: end-to-end SOP.
- `references/replace-with-your-ip.md`: how users replace the sample IP with their own character.
- `references/style-variants.md`: style selection system.
- `references/prompt-templates.md`: reusable prompt blocks.
- `references/quality-checklist.md`: validation rules.
- `references/examples.md`: worked examples.
- `assets/cover-brief-template.md`: copyable brief template.
- `assets/ip-character-card-template.md`: copyable IP character card template.
