---
name: frontend-design
description: Use whenever building an interactive HTML module, simulation, game, matching activity, or any student-facing digital artefact as a single file.
---

# Building Educational Interactives

This skill governs how Claude builds interactive HTML modules for classroom use. The goal is always a working, self-contained file a teacher can publish directly to GitHub Pages and a student can open on a phone.

## Non-negotiable constraints

Every interactive must meet all of these before being considered complete:

- Single HTML file. CSS and JavaScript live inside it. No external libraries, no CDN links, no dependencies. The file must work if saved to a desktop and opened without internet.
- Mobile-first. Assume a 375px-wide screen. Touch targets at least 44px. No hover-only interactions.
- No login, no data collection, no cookies. Students open it and use it. Nothing is stored.
- Works offline once loaded. No fetch calls to external APIs.

## Audience defaults for Singapore primary classes

Unless told otherwise, assume:
- Students are aged 9 to 12.
- A third of the class may have English as a second language. Use short sentences, concrete nouns, and familiar Singapore examples (durian, hibiscus, HDB block, MRT). Avoid idioms.
- Four to five students may need scaffolding. Build in visible hints or simplified modes where possible.
- The interactive will be used on a school device or personal phone during class time. Assume 20 to 30 minutes of use maximum.

## Code quality

- Semantic HTML5. Use `<button>`, `<label>`, `<section>`, `<main>`. Do not use `<div>` for interactive elements.
- WCAG AA colour contrast minimum. Never put light text on a light background.
- No inline event handlers (`onclick=""`). Use `addEventListener`.
- Functions named for what they do: `checkAnswer()`, `resetGame()`, not `fn1()`.
- CSS variables for colours at the top of the style block. Makes theming easy.

## Before building

If the prompt is ambiguous on any of these, ask one clarifying question before writing a line of code:
- What misconception or learning objective is this targeting?
- What does correct look like? What does a wrong answer reveal?
- Should there be a score, a timer, or neither?
- What happens when the student finishes: replay, summary, or just done?

Do not ask more than one question. If several things are unclear, pick the most important one.

## What to do

- Announce what you are building before you write the code: one sentence summary, the interaction type, and the target misconception.
- Write the full file, not a fragment. If it is long, write it in one block.
- After the code, add three lines: what the file does, how to publish it to GitHub Pages, and one suggestion for how to extend it next.

## What to avoid

- Do not use React, Vue, Bootstrap, jQuery, or any framework. Vanilla HTML, CSS, and JavaScript only.
- Do not add sound effects, auto-playing media, or animations that cannot be paused.
- Do not use red and green as the only indicators of correct and wrong. Some students are colour-blind. Add an icon or text label too.
- Do not make the interaction so open-ended that there is no clear correct state. Every interactive needs a moment of resolution the student can feel.
- Do not write placeholder content ("Lorem ipsum", "Question 1 here"). If you do not have real content, ask for it.
