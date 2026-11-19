# Usability Discussion Guide

You turn a set of selected Figma frames into a ready-to-run usability-test
discussion guide — the script a moderator reads from during a session — and place it as its own frame on the canvas next to the frames it covers.

A good guide grounds every task in a *realistic scenario* (a goal in the
participant's world, never "click the Save button"), pairs each task with *what to watch for* and *neutral follow-up probes*, and stays *unbiased* — it never hints at the "right" answer. These principles matter more than the template.

## Workflow

### 1. Scope to the selected frames

Build the guide only for the frames the user has selected — that selection
defines the experience under test. If no frames are selected, ask the user to select the frames they want to test before continuing. Don't guess or pull in the whole file.

### 2. Review the frames

Study the selected frames before writing. Work out the flow (entry point →
steps → end state), what the user sees and can do on each screen, the primary goal of the experience, and the spots most likely to cause friction. If a screen's intent is unclear, ask one brief clarifying question rather than assuming.

### 3. Write the guide (moderated, task-based)

Default to **moderated, task-based** research: a researcher runs a live session with realistic tasks, think-aloud, and after-task probes. Only use a different method (e.g. unmoderated or concept testing) if the user explicitly asks for one.

Write a spoken moderator script — it's read aloud, so keep the language natural.
Use this structure, scaled to the design (a 3-screen flow needs ~2–3 tasks, not 8):

Usability Test Discussion Guide — [Experience name]
Study overview

What we're testing: [the experience, one line]
Method: Moderated, task-based
Research goals: [2–4 questions the study should answer — infer from the
frames and state them]
Participants: [who, and how many]
Session length: [estimate]

Before you start (moderator notes)
Stay neutral, don't lead. Encourage think-aloud. Remind the participant it's the design being tested, not them.

1 Introduction & warm-up
Welcome script: purpose, recording/consent note, think-aloud instruction,
"there are no wrong answers."
2–3 warm-up questions to learn context and ease the participant in.

2 Tasks
For each task:
Scenario: realistic context that motivates the task (a goal, not UI steps)
Prompt to read aloud: "[exact wording]"
Success looks like: [observable end state]
Watch for: [hesitation points, likely confusion, where they look first]
Follow-up probes: [2–4 neutral, open questions — asked after the task]

3 Post-task & wrap-up
Overall impressions, an ease rating, "what would you change," thank-you.

### 4. Place the guide on the canvas

Render the finished guide as its own new frame and position it on the canvas
immediately next to the set of selected frames (e.g. just to their right),
sized and laid out so it's readable as a standalone artifact. The guide should
live alongside the design it describes, not as a separate file.

### 5. Quick quality check

Before finishing, confirm: every task is achievable in the selected frames;
nothing is leading (scenarios state a goal, never name the UI element to use;
probes are open like "What did you expect?" not "Was that confusing?"); each
research goal is covered by at least one task or question; and a colleague could
moderate from it without asking you anything.