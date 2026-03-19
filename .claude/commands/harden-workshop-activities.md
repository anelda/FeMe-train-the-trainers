Read the input file carefully. This is a workshop activities file (typically `workshop-activities.md`).

$ARGUMENTS

## Step 1: Load the outcomes map

Find and read `outcomes-map.md` in the same directory as the input file. This contains the learning outcomes, their Bloom's taxonomy levels, and the exercise-to-outcome mappings.

If `outcomes-map.md` does not exist, stop and tell the user to run `/harden-outcomes` first.

### Bloom's taxonomy levels (for reference)

1. **Remember** — recall facts or concepts (verbs: define, list, name, identify, describe)
2. **Understand** — explain ideas or concepts (verbs: explain, summarise, paraphrase, classify, discuss)
3. **Apply** — use information in new situations (verbs: apply, demonstrate, use, implement, solve)
4. **Analyse** — draw connections among ideas (verbs: analyse, compare, contrast, examine, differentiate)
5. **Evaluate** — justify a decision or judgement (verbs: evaluate, justify, critique, assess, argue)
6. **Create** — produce new or original work (verbs: create, design, develop, formulate, construct)

## Step 2: Map each workshop activity to an outcome

For each activity in the input file:

1. **Identify what the activity actually asks participants to do.** Look at the instructions, not just the title. What is the core cognitive task?
2. **Classify the activity's Bloom's level** based on that core task.
3. **Match it to the most relevant outcome** from the outcomes map.
4. **Compare Bloom's levels** between the activity and its matched outcome.

## Step 3: Build an alignment report

Your report should be saved to to `workshop-activities-outcomes-map.md`

Present your findings in this format:

```
## Workshop Activity Alignment Report

### Activity [N]: [Title]
- **What participants do:** [one-sentence summary of the core cognitive task]
- **Activity Bloom's level:** [level]
- **Matched outcome:** [outcome text]
- **Outcome Bloom's level:** [level]
- **Alignment:** MATCH | ACTIVITY EXCEEDS OUTCOME | ACTIVITY UNDERSHOOTS OUTCOME | NO MATCHING OUTCOME

[If mismatched or unmatched, explain the issue in one or two sentences.]
```

After all activities, add:

```
### Unmatched outcomes

List any outcomes from the outcomes map that have no corresponding workshop activity. Note: not every outcome needs a workshop activity — this is informational, not necessarily a problem.

### Summary

- [N] activities aligned
- [N] activities exceed their outcome
- [N] activities undershoot their outcome
- [N] activities with no matching outcome
- [N] outcomes with no workshop activity
```

## Step 4: Suggest specific changes

For each misalignment, suggest **one concrete fix**. Prefer the smallest change that resolves the issue. Options to consider:

- **Activity undershoots outcome:** Add a step that raises the cognitive demand. Be specific — write the actual step to add or modify.
- **Activity exceeds outcome:** Usually fine for a workshop (stretch is good in facilitated settings). Only flag if the gap is large (two or more Bloom's levels apart). If flagging, suggest either simplifying the activity or note that the outcome could be levelled up.
- **Activity has no matching outcome:** Suggest which outcome it could serve with a small tweak, or flag it as a candidate for removal.
- **Outcome has no workshop activity:** Only suggest adding a new activity if the outcome is central to the chapter and has no self-study exercise covering it either. Workshop time is limited — not every outcome needs a live activity.

For each suggestion, write the specific change — the actual revised instruction step, the rephrased debrief question, or the new activity skeleton. Do not be vague ("make it more demanding") — show what you mean.

## Step 5: Ask the user

Present the alignment report and your suggestions. Ask the user which changes (if any) they want you to make. Do NOT edit the input file until the user approves.

## Step 6: Apply approved changes

Edit the workshop activities file with only the approved changes. Preserve the existing format, tone, and structure. Use the **voice-and-tone** skill for any new or rewritten text.

## Step 7: Update the workshop activity alignment report

Do NOT edit `outcomes-map.md` — that file maps self-study exercises to outcomes and is managed by `/harden-outcomes`.

Instead, save the alignment report from Step 3 (updated to reflect any changes made in Step 6) to `workshop-activities-outcomes-map.md` in the same directory as the input file. This is the workshop-specific equivalent of the outcomes map.
