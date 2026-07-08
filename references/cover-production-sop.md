# Cover Production SOP

## Purpose

Use this SOP to produce Xiaohongshu cover images with a repeatable personal IP character system. The goal is not only to make one nice cover, but to create a visual pattern that can be reused across a creator's content calendar.

## Step 1: Collect the Brief

Collect or infer:

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

Defaults:

```text
Aspect ratio: 3:4
Cover type: Xiaohongshu knowledge cover
Style: high-contrast sticker collage
Character mode: choose by content type
Style variant: choose by topic
```

Success criteria:

- The main title is short enough to read in a feed.
- The reader promise is specific.
- The topic can be explained in one sentence.

## Step 2: Choose Character Mode

Choose a mode by content type:

| Content type | Character mode | Reason |
|---|---|---|
| Method explainer | Professional mode | Builds trust and authority |
| Tool tutorial | Professional mode | Signals practical workflow value |
| Case study | Professional mode | Feels like real project review |
| Product or course promotion | Professional mode | Avoids looking too playful |
| Beginner explainer | Friendly mascot mode | Reduces learning pressure |
| Resource recommendation | Friendly mascot mode | Feels like a friend sharing favorites |
| Gentle warning | Friendly mascot or professional mode | Use mascot for soft warnings, professional for serious warnings |
| Opinion | Depends on tone | Warm opinions use mascot; strong claims use professional mode |

## Step 3: Choose Style Variant

Pick a variant by the cover's role:

| Need | Recommended variant |
|---|---|
| Make beginners feel safe | Cream Companion |
| Make tools feel efficient | Black Efficiency |
| Make process feel executable | Utility Fieldwork |
| Make a hook feel urgent | Street Sprint |

If uncertain, choose Utility Fieldwork for workflow/case content, Cream Companion for beginner content, and Black Efficiency for tool lists.

## Step 4: Build the Cover Structure

Recommended structure:

```text
Top: small content tag
Upper-middle: oversized main title
Middle: process cards, tool cards, or sticker information blocks
Lower-right or lower-middle: personal IP character
Bottom: account positioning or reader benefit tag
```

Recommended proportions:

- Title: 35% to 45% of the canvas.
- Character: 30% to 40% of the canvas.
- Information blocks: 3 to 5 blocks.

Success criteria:

- The title is the first thing seen.
- The character supports recognition without stealing the title.
- The cover has one visual protagonist.

## Step 5: Write the Generation Prompt

Use this structure:

```text
Create a Xiaohongshu cover image, vertical 3:4, polished commercial illustration style.

Topic: [topic]
The main title must be large, clear, and readable: [main title]

Main character:
[character mode description]

Character action:
[action]

Layout:
[layout description]

Visual elements:
[cards, stickers, arrows, icons, screenshots, notes]

Text hierarchy:
Top tag: [tag]
Main title: [main title]
Bottom tag: [tag]

Constraints:
Readable in mobile feed.
No watermark.
No real brand logo unless provided by the user.
No unrelated props.
No extra people.
No garbled text.
No long English paragraphs.
```

## Step 6: Generate One Direction First

For a new cover system, generate one direction first. Do not batch too many images before the user validates the direction.

Evaluate only:

- Title impact
- Character mood
- Style fit
- Series potential

Do not over-focus on tiny text or perfect character consistency in the first exploration.

## Step 7: Run Checks

Run three checks:

1. Thumbnail check: title and topic are readable in a small mobile feed.
2. Character check: the IP character remains recognizable.
3. Information check: every sticker/card supports the topic.

Use `quality-checklist.md` for details.

## Step 8: Iterate

If the title is weak:

1. Enlarge the title.
2. Reduce stickers.
3. Increase contrast.
4. Split the title into two lines.

If the character is inconsistent:

1. Strengthen fixed facial traits.
2. Strengthen clothing/hat traits.
3. Use the user's character reference image.
4. Reduce complex gestures.

If the cover feels childish:

1. Keep the mascot element but reduce toy-like clothing.
2. Add process cards, tool cards, screenshots, or project-board elements.
3. Use cleaner black/white/yellow/blue contrast.
4. Reduce candy colors.

If the cover is messy:

1. Keep only three information blocks.
2. Add whitespace.
3. Use consistent stroke width.
4. Remove decorative stickers that do not explain the topic.

## Step 9: Archive

Archive explorations separately from final covers.

Suggested structure:

```text
assets/ip-character/[character-name]/style-tests/
assets/ip-character/[character-name]/references/
covers/YYYY-MM-DD-[topic]/output/
```

For Obsidian vaults:

```text
素材库/IP形象/[角色名]/
草稿/YYYY/小红书/[主题]-social-card/output/
```

For each style-test folder, include a note recording:

- Style name
- Suitable content
- Visual keywords
- Reuse prompt
- Whether it should become a long-term style

