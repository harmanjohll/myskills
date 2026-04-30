# Slash Commands

Paste each prompt body into: **claude.ai → Settings → Customize → Add slash command**
Name it exactly as shown (without the `/`). The skill referenced must already be uploaded to your account.
---
## frontend-design

### `/build-interactive`
```
Build an interactive HTML [simulation / game / matching activity] on [topic] for [year level]. Apply the frontend-design skill. Ask me one clarifying question before writing any code.
```
### `/debug-interactive`
```
Review this HTML file and identify any issues with accessibility, mobile layout, or code quality. Apply the frontend-design skill.
```
*(Paste your HTML into the chat after the command fires.)*
---
## my-class-context
### `/lesson-plan`
```
Plan a 45-minute lesson on [topic]. Use the my-class-context skill. Structure: hook, surface misconception, exploration, resolution, exit ticket. Include timings and one sentence-stem I can use at each phase.
```
### `/diagnostic`
```
Write one diagnostic question on [topic] that surfaces the most common misconception. Give me four answer options and tell me what each wrong answer reveals about a student's thinking. Use the my-class-context skill.
```
---
## teacher-voice
### `/parent-letter`
```
Draft a parent letter about [topic or event]. Apply the teacher-voice skill. Ask me for any specific details before drafting.
```
### `/report-comment`
```
Write an end-of-term report comment for a student who [three notes about the student]. Keep it specific, avoid clichés, match a warm professional register. Apply the teacher-voice skill.
```
### `/staff-memo`
```
Draft a staff memo about [decision or request]. Keep it under 150 words. Apply the teacher-voice skill.
```
---
## learning-ux
### `/ux-audit`
```
Audit this resource for learning UX issues. Apply the learning-ux skill. List problems first, then propose fixes.
```
*(Paste your resource or describe it after the command fires.)*
### `/ux-redesign`
```
Redesign this resource with learning UX principles applied. Apply the learning-ux skill. State each UX decision you are making before producing the output.
```
*(Paste your resource after the command fires.)*
---
## Combined (use when both skills should fire together)
### `/build-lesson-interactive`
```
Build an interactive HTML [simulation / game / matching activity] on [topic]. Apply both the frontend-design skill and the learning-ux skill. Before building: name the one thing a student must successfully do, identify the highest cognitive load moment, and ask me one clarifying question. Then build.
```
---
## Notes
- Replace anything in `[square brackets]` with your specifics before running.
- Commands that say *"paste after"* fire the prompt first, then you paste the content in the same message or the next one.
- A slash command can reference a skill by name in its body. Claude will load the skill even if the automatic trigger does not fire.
- To check which skill loaded: type `"Which skill did you load for that?"` after any response.
