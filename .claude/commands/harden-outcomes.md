Read over the input file carefully.

$ARGUMENTS

## Step 1: Create outcomes-map.md

Create a file called `outcomes-map.md` in the same directory as the input file. This file maps every learning outcome to the exercises that address it, and vice versa — including the Bloom's taxonomy level of each.

### Bloom's taxonomy levels (for reference)

1. **Remember** — recall facts or concepts (verbs: define, list, name, identify, describe)
2. **Understand** — explain ideas or concepts (verbs: explain, summarise, paraphrase, classify, discuss)
3. **Apply** — use information in new situations (verbs: apply, demonstrate, use, implement, solve)
4. **Analyse** — draw connections among ideas (verbs: analyse, compare, contrast, examine, differentiate)
5. **Evaluate** — justify a decision or judgement (verbs: evaluate, justify, critique, assess, argue)
6. **Create** — produce new or original work (verbs: create, design, develop, formulate, construct)

### Classifying outcomes and exercises

- **Each outcome** should contain (or clearly imply) a verb from one of the Bloom's levels above. Identify which level it targets. If the outcome verb is vague or missing (e.g. "know about", "be familiar with"), flag it as **⚠️ VAGUE VERB** — it needs a sharper action verb.
- **Each exercise** also operates at a Bloom's level based on what it actually asks the learner to *do*. Identify that level.

### Format

Use this format:

```
# Outcomes Map

## Outcomes → Exercises

For each learning outcome listed in the input file, list it below with its Bloom's level and the exercises that address it. If an outcome has NO matching exercise, mark it with **⚠️ UNMET**.

### Outcome 1: [outcome text]
- **Bloom's level:** [level] (verb: [the verb in the outcome])
- **Exercise:** [exercise name] — Bloom's level: [level]
- **Exercise:** [exercise name] — Bloom's level: [level]

### Outcome 2: [outcome text]
- **Bloom's level:** [level] (verb: [the verb in the outcome])
- **⚠️ UNMET** — no exercise directly addresses this outcome.

(...and so on for every outcome)

## Exercises → Outcomes

For each exercise/activity in the input file, list it below with its Bloom's level and the outcomes it serves. If an exercise does NOT clearly serve any outcome, mark it with **⚠️ ORPHAN**.

### Exercise: [exercise name]
- **Bloom's level:** [level] (based on what the learner actually does)
- **Serves outcome:** [outcome text] — Outcome Bloom's level: [level]

### Exercise: [exercise name]
- **Bloom's level:** [level]
- **⚠️ ORPHAN** — this exercise does not clearly serve any listed outcome.

(...and so on for every exercise)

## Bloom's Alignment Issues

For each outcome–exercise pair, compare the Bloom's levels. Flag mismatches:

- **⚠️ EXERCISE EXCEEDS OUTCOME** — the exercise asks learners to operate at a *higher* Bloom's level than the outcome requires (e.g. exercise asks them to *apply* but the outcome only says *understand*). Suggestion: level up the outcome verb, or simplify the exercise.
- **⚠️ EXERCISE UNDERSHOOTS OUTCOME** — the exercise operates at a *lower* Bloom's level than the outcome claims (e.g. outcome says *evaluate* but the exercise only asks them to *remember*). Suggestion: make the exercise more demanding, or be honest and lower the outcome.

## Flags for Review

List all issues found:
- Unmet outcomes (with suggestions: adjust an existing exercise, add a new one, or relax the outcome)
- Orphan exercises (with suggestions: link to an outcome, adjust, or remove)
- Exercises that only weakly address an outcome
- Vague outcome verbs (with suggested replacement verbs)
- Bloom's level mismatches between outcomes and their exercises (with suggestions to level up or level down)
```

Every outcome and every exercise from the input file must appear in the map. Do not skip any.

## Step 2: Review the map critically

Read over the outcomes-map.md you just created. For each flag:

- **Unmet outcomes:** Could an existing exercise be tweaked to cover it? Should a new exercise be added? Or is the outcome too ambitious and should be reworded or removed?
- **Orphan exercises:** Do they serve a purpose that is not captured by the current outcomes? Should an outcome be added, or should the exercise be cut?
- **Weak links:** Are there exercises that technically touch an outcome but do not give learners enough practice to actually meet it?
- **Vague verbs:** Suggest a specific Bloom's-aligned verb to replace the vague one.
- **Bloom's mismatches:** For each mismatch, recommend whether to level up the outcome, level down the exercise, or both. Be specific — suggest the new verb or the change to the exercise.

Present your suggestions clearly in the Flags for Review section but do NOT make changes to the input file yet. Wait for the user to review.

## Step 3: Ask the user

Present a summary of the flags and your suggestions. Ask the user which changes (if any) they want you to make to the input file.

## Step 4: Apply approved changes

If the user approves changes, update the original input file. Only change what was approved.

## Step 5: Final read-through

In a sub agent:

Read over the whole input file one more time and check that:
- Every outcome now uses a clear Bloom's-aligned verb
- Every exercise aligns with (or deliberately stretches beyond) its outcome's Bloom's level
- Exercises make sense in context (not too hard, not too easy for the target audience)
- The flow from prose to exercise feels natural
- Exercise instructions are clear enough that a reader could actually do them
- Nothing feels redundant or out of place after the edits

Flag anything that still feels off and suggest fixes.
