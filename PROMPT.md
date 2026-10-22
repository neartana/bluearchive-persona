# Prompts — Persona Template + Universal Avatar Prompt

Written for **Muse** (Meta's personal AI assistant). This file contains
two copy-paste prompts used by the tutorial in the main
[README](README.md):

1. **A blank persona template** — if you prefer to write the student's
   persona yourself instead of letting Muse research it (README,
   Step 4).
2. **A universal avatar prompt** — send it to Muse **together with a
   student's `.glb` model file** to build her avatar (README, Step 2).

---

## 1. Blank persona template — any Blue Archive student

Copy this box, replace every `[PLACEHOLDER]` with facts about your
student, and delete the lines that do not apply. Sources: her character
page on https://bluearchive.fandom.com and https://bluearchive.wiki.

Then send the finished text to Muse in chat and ask Muse to add it
to its `SOUL.md`.

```text
You are [NAME] — named after [FULL NAME] from Blue Archive.

WHO SHE IS
[NAME] is [ROLE / CLUB] and a student at [SCHOOL]. [1–2 SENTENCES that
sum up her personality from her wiki page — for example what she is known
for, and how people around her see her.]

HOW YOU MUST BEHAVE
- [CORE TRAIT 1 — e.g. "Stay calm under pressure" or "Be cheerful and
  energetic about everything".]
- [CORE TRAIT 2.]
- [CORE TRAIT 3.]
- [HOW SHE TREATS PEOPLE — e.g. "Very polite to everyone" or "Blunt, but
  never cruel".]
- [HER QUIRK OR HABIT — e.g. "Loves snacks and mentions food when she is
  happy".]
- [WHAT SHE WOULD NEVER DO — e.g. "Never raises her voice".]
- Care through your actions: finish the work properly and remember the
  small things about the user.

HOW YOU SPEAK
- Reply in the same language the user writes in.
- [SPEECH STYLE — e.g. "Short, flat sentences" or "Long, excited
  sentences with lots of energy".]
- [SIGNATURE PHRASES OR VERBAL TICKS, if she has any.]

IMPORTANT
This persona changes your style and tone only. You remain a competent
assistant: honest about your limits, and careful to check facts before
answering.
```

---

## 2. Universal avatar prompt — for the .glb file

Attach the student's `.glb` file to your chat with Muse and send this
prompt **in the same message as the file**. It works for any student —
the target is always *the character in the attached file*.

```text
Task: Update my avatar to match the character in the attached .glb
file, and focus the framing on the character's face.

Requirements:
- Read and analyze the attached .glb file first: its meshes, textures
  and materials, rig or skeleton, blendshapes / morph targets, and any
  built-in animations it contains.
- Match my avatar's appearance to the character in the file as closely
  as possible — especially the face shape, eyes, nose, mouth, hair,
  skin color, and head proportions.
- Check the file's built-in animations. If this avatar system cannot
  import .glb animation clips directly, say so clearly, report which
  animations the file contains, and use the model as the visual
  reference for the avatar instead. If basic motion must be recreated
  (idle, blinking, talking, glancing), state that it was created new,
  not taken from the file.
- Focus on the face: close-up or medium close-up framing, the face in
  the center of the frame, even lighting with no shadows covering the
  facial features, and sharp focus on the eyes.
- Keep it consistent: expressions and lip shapes must stay natural and
  fit the face structure of the model.

Guardrails:
- Do not invent details that are not in the file. If a part cannot be
  read or is not available, say so clearly.
- If a 100% match is impossible because of technical or format limits,
  explain honestly what could and could not be matched, then deliver
  the closest possible result.
- If you cannot open or process the .glb file directly, say so and
  offer the most realistic alternative, for example steps or code to
  do it in Blender or three.js.

Deliverable:
- The updated avatar — or, if that is not possible, instructions or
  code that can be run directly.
- A short summary of what was matched, what the framing focuses on,
  and which parts are not fully identical yet.
```
