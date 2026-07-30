---
name: visualize-this-slide-editable
description: Use when I ask Copilot in PowerPoint to visualize, redesign, transform, or improve a selected slide like visualize-this-slide, but the result must be built with editable PowerPoint objects instead of a flattened image. Create native text boxes, shapes, icons, lines, tables, charts, SmartArt-like layouts, and editable diagrams that follow the existing deck design.
---
# Visualize This Slide With Editable PowerPoint Objects

Use this skill when the user wants to convert a text-heavy, plain, or unclear slide into a polished visual slide while keeping the output editable in PowerPoint.

The goal is similar to `visualize-this-slide`, but the output must **not** be a single non-editable image. Instead, create the visual using native PowerPoint objects so the user can edit text, colours, shapes, positions, sizes, connectors, icons, charts, and tables afterwards.

## Core principles

1. **Use editable PowerPoint objects only for the main visual.**
   - Prefer text boxes, placeholders, shapes, lines, connectors, icons, tables, charts, SmartArt-style arrangements, grouped objects, and theme-aware formatting.
   - Do not replace the slide with one large raster image.
   - Do not insert a screenshot of the designed slide as the final output.

2. **Preserve the original meaning.**
   - Keep the user's current message, storyline, claims, facts, terms, key numbers, and labels.
   - Compress or rephrase only when it improves clarity and does not change meaning.
   - Do not invent facts, metrics, product names, dates, customers, or claims.

3. **Respect the deck style.**
   - Analyse the existing slide and nearby slides for theme colours, fonts, spacing, title style, shapes, icons, and visual density.
   - Use the current deck theme and layouts where possible.
   - Match the visual tone of the deck rather than introducing an unrelated style.

4. **Make everything easy to edit.**
   - Keep important text in editable text boxes or placeholders.
   - Use individual shapes for cards, steps, pillars, nodes, timelines, callouts, badges, and background panels.
   - Group related objects only when grouping makes later editing easier. Avoid over-grouping the entire slide.
   - Use clear selection order and sensible object layering.

5. **Prefer clean business visuals.**
   - Use a simple structure with strong hierarchy.
   - Reduce clutter.
   - Use alignment, whitespace, contrast, and consistent sizing.
   - Use accessible colour contrast and readable font sizes.

## Workflow

### 1. Understand the selected slide

Review the selected slide and identify:

- The core message of the slide.
- The key points, evidence, or steps.
- Any existing hierarchy, such as title, subtitle, sections, bullets, data, or callouts.
- Any brand or template constraints visible in the deck.
- Whether the information is best shown as a process, timeline, comparison, framework, matrix, cycle, funnel, architecture, dashboard, roadmap, table, chart, or set of cards.

If the slide already contains a clear visual structure, improve it rather than fully replacing it.

### 2. Choose an editable visual pattern

Select one primary visual pattern based on the content:

- **Process or sequence:** editable timeline, numbered steps, flow, swimlane, or chevron progression.
- **Comparison:** editable two-column compare/contrast, scorecard, pros/cons, matrix, or before/after layout.
- **Strategy or framework:** editable pillars, flywheel, layered model, pyramid, hub-and-spoke, or quadrant.
- **Data or metrics:** editable chart, data cards, KPI strip, table, or labelled callouts.
- **Architecture or workflow:** editable system diagram using containers, nodes, arrows, connectors, and labels.
- **Problem and solution:** editable split layout with pain points, solution blocks, and outcome callouts.
- **Agenda or summary:** editable cards, section tiles, or chapter roadmap.

Use only one dominant pattern unless the slide clearly needs a small supporting element, such as a KPI strip above a process.

### 3. Create the editable slide

Transform the slide using native objects:

1. Keep or improve the slide title.
2. Convert dense bullets into concise labels, cards, diagram nodes, or callouts.
3. Place supporting details in smaller editable text boxes.
4. Use editable shapes for visual containers and emphasis.
5. Add editable connectors or arrows when showing relationships or flow.
6. Use editable tables or charts for structured data.
7. Use vector icons or simple shape-based icons when helpful.
8. Align and distribute objects precisely.
9. Keep margins consistent with the deck.
10. Use theme colours, fonts, and styles from the presentation.

### 4. Avoid non-editable outputs

Do **not** do any of the following unless the user explicitly asks for an image:

- Do not generate a full-slide illustration and place it as a background.
- Do not flatten native objects into a PNG/JPEG/SVG screenshot.
- Do not use a single image to represent a process, timeline, framework, or architecture diagram.
- Do not use image-only text, because the user cannot edit it later.

If decorative imagery is needed, keep it secondary and ensure the main information remains editable.

### 5. Quality check before finishing

Before finalising the slide, check that:

- The slide's main message is clearer than before.
- All essential slide content is retained or accurately condensed.
- The final slide follows the existing deck's visual style.
- The main visual is made from editable PowerPoint objects.
- Text is readable in presentation mode.
- The layout has balanced spacing and alignment.
- The slide does not contain one large flattened image.
- The user can select and edit individual components.

## Response behaviour

After applying the skill, briefly tell the user what visual pattern was used and confirm that the slide was built with editable PowerPoint objects.

Example response:

> I redesigned the selected slide as an editable three-step process diagram using native PowerPoint shapes, text boxes, connectors, and theme colours, so you can adjust every element afterwards.

## Example user prompts that should trigger this skill

- `@visualize-this-slide-editable improve this slide visually but keep everything editable.`
- `Visualize this slide using PowerPoint objects instead of an image.`
- `Turn this bullet slide into an editable diagram.`
- `Make this slide look like visualize-this-slide, but don't flatten it into an image.`
- `Create an editable visual version of the current slide.`
- `Convert this slide into editable shapes, icons, and text boxes.`

## Edge cases

- If the selected slide contains a chart or table, keep it editable and improve formatting rather than converting it into an image.
- If the slide contains detailed numeric data, preserve values exactly unless the user asks for summarisation.
- If there is too much content for one slide, create a cleaner visual summary on the current slide and move secondary details into speaker notes only if PowerPoint supports that action in the current context.
- If the slide is already visual, refine hierarchy, alignment, readability, and styling without unnecessary redesign.
- If the user asks for photorealistic imagery, clarify through the output that any decorative image would not be editable, and keep core information in editable objects.
