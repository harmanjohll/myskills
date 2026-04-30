---
name: learning-ux
description: Use whenever designing the layout, flow, or user experience of any student-facing resource — digital or print — including interactives, worksheets, slides, and assessment tools.
---

# Learning UX

This skill governs how Claude thinks about the experience of the learner, not just the accuracy of the content. A resource can be factually correct and pedagogically sound and still fail because a student cannot navigate it, is overwhelmed by it, or does not know what to do next.

When this skill is loaded, Claude considers UX before producing anything. Content and UX are designed together, not in sequence.

## The five questions Claude asks before building

1. **What is the one thing a student must successfully do here?** Everything else is secondary. Name it.
2. **What does a confused student look like at each step?** Build for that student, not the student who already understands.
3. **What does correct feel like?** Success must be perceptible, not just technically registered.
4. **What is the heaviest cognitive load moment?** Redesign that moment first.
5. **What happens when a student is done?** There must be a clear ending, not a page that just sits there.

## Principles

**One thing at a time.** Do not present all information simultaneously. Reveal it in the order the learner needs it. Instructions appear before the task. Feedback appears after the attempt, not before.

**Visible progress.** Students should always know where they are, what comes next, and roughly how far they have left. A progress indicator, a step count, or a simple "Question 3 of 5" is enough.

**Forgiving errors.** A wrong answer is information, not a failure. Feedback on incorrect responses should tell the student what to try differently, not just that they were wrong. "Not quite — think about what the plant needs, not what it produces" beats "Incorrect."

**Reduce reading load.** Every word on screen costs attention. If a sentence can be cut, cut it. Labels over paragraphs. Diagrams over labels where possible. Never put instructions and the task on the same visual level.

**One obvious next step.** At every moment, there is one thing the student should do. Make it visually dominant. A button they cannot miss. A field that is clearly waiting for input. Never leave the student wondering what to do.

**Low stakes feel.** The interface should feel safe to try, fail, and try again. Avoid scoring language that frames every mistake as a loss. "Try again" beats "Wrong." "Nice — here's what's happening" beats a score counter that ticks down.

## Application by format

**Digital interactives:** Limit to one interaction type per screen. Show the question before revealing the answer choices. Animate transitions only if they carry meaning (e.g. a leaf growing as conditions improve). Never auto-advance without student action.

**Worksheets and print resources:** Leave more white space than feels comfortable. Group related items visually. Use one font size for questions, a clearly different size for instructions. Number steps explicitly, even if the order seems obvious.

**Slides and presentations:** One idea per slide. Title states the idea, not the topic. Body illustrates or evidences it. No bullet points that the teacher will read aloud word for word.

**Assessment tools:** Separate reading load from thinking load. A question that requires understanding a long passage AND a complex concept is testing two things at once. Test one.

## What to do

- State the UX decisions you are making before producing the resource. "I am putting the instructions above the input field because students need to read them before they can act."
- Flag any moment where the cognitive load is high and propose a way to reduce it.
- When given an existing resource to improve, list the UX issues first, then fix them. Do not silently rewrite.

## What to avoid

- Do not make UX decisions invisible. Name them so the teacher understands and can override.
- Do not add features that serve the designer rather than the learner: animations for aesthetics, sound effects for atmosphere, complexity for impressiveness.
- Do not assume a student will read the instructions. Design for the student who skips them.
- Do not end a resource with a blank screen. Every resource needs a clear endpoint: a summary, a prompt to share with a partner, or a simple "You're done."
